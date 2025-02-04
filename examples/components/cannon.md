# Cannon

The Cannon component allows Cannon2 and Cannon3 to become functional networked cannons. Do not use this on any other objects.

```csharp
component Cannon
{
    UnlimitedAmmo = true;
    MaxAmmo = 0;
    Cooldown = 3.0;
    _rotateSpeed = 20;
    _ballSpeed = 300.0;
    _barrel = null;
    _humanMount = null;
    _barrelEnd = null;
    _inUse = false;
    _cooldownLeft = 0.0;
    _ammoLeft = 0;
    _human = null;
    _collidingHuman = null;

    function Init()
    {
        self._barrel = self.MapObject.GetTransform("Barrel");
        self._barrelEnd = self._barrel.GetTransform("End");
        self._humanMount = self.MapObject.GetTransform("HumanMount");
        self.MapObject.AddSphereCollider("Region", "Characters", Vector3.Zero, 15.0);
        self._ammoLeft = self.MaxAmmo;
    }

    function SendNetworkStream()
    {
        self.NetworkView.SendStream(self._barrel.LocalRotation);
        self.NetworkView.SendStream(self._inUse);
        self.NetworkView.SendStream(self._ammoLeft);
    }

    function OnNetworkStream()
    {
        rotation = self.NetworkView.ReceiveStream();
        self._barrel.LocalRotation = rotation;
        self._inUse = self.NetworkView.ReceiveStream();
        self._ammoLeft = self.NetworkView.ReceiveStream();
    }

    function OnNetworkMessage(sender, message)
    {
        if (Network.IsMasterClient && self.NetworkView.Owner == Network.MyPlayer && !self._inUse && message == "request")
        {
            self.NetworkView.Transfer(sender);
        }
    }

    function OnNetworkTransfer(oldOwner, newOwner) 
    {
        if (newOwner == Network.MasterClient && Network.IsMasterClient)
        {
            self._inUse = false;
            self.ResetBarrel();
        }
        elif (newOwner == Network.MyPlayer)
        {
            self._inUse = true;
            human = Network.MyPlayer.Character;
            if (human != null && human.Type == "Human")
            {
                human.MountTransform(self._humanMount, Vector3.Zero, Vector3.Zero);
                self._human = human;
            }
        }
    }

    function OnCollisionStay(other)
    {
        if (other.Type == "Human" && other.IsMine && !self._inUse)
        {
            UI.SetLabelForTime("MiddleCenter", "Press " + Input.GetKeyName("Interaction/Interact") + " to use cannon.", 0.1);
            self._collidingHuman = other;
        }
    }

    function OnTick()
    {
        self._collidingHuman = null;
    }

    function OnFrame()
    {
        if (self._inUse && self.NetworkView.Owner == Network.MyPlayer)
        {
            self._cooldownLeft = self._cooldownLeft - Time.FrameTime;
            message = "Cooldown: " + Convert.ToString(Convert.ToInt(Math.Clamp(self._cooldownLeft, 0.0, self.Cooldown)));
            if (!self.UnlimitedAmmo)
            {
                message = message + " Ammo: " + Convert.ToString(self._ammoLeft);
            }
            UI.SetLabelForTime("MiddleCenter", message, 0.1);
            barrelRotation = self._barrel.LocalRotation;
            baseRotation = self.MapObject.Rotation;
            if (Input.GetKeyHold("General/Left"))
            {
                baseRotation.Y = baseRotation.Y - self._rotateSpeed * Time.FrameTime;
            }
            elif (Input.GetKeyHold("General/Right"))
            {
                baseRotation.Y = baseRotation.Y + self._rotateSpeed * Time.FrameTime;
            }
            if (Input.GetKeyHold("General/Forward"))
            {
                barrelRotation.X = barrelRotation.X - self._rotateSpeed * Time.FrameTime;
            }
            elif (Input.GetKeyHold("General/Back"))
            {
                barrelRotation.X = barrelRotation.X + self._rotateSpeed * Time.FrameTime;
            }
            barrelRotation.X = Math.Clamp(barrelRotation.X, -45.0, 45.0);
            self._barrel.LocalRotation = barrelRotation;
            self.MapObject.Rotation = baseRotation;
            hasAmmo = self._ammoLeft > 0 || self.UnlimitedAmmo;
            if (self._cooldownLeft <= 0.0 && hasAmmo && Input.GetKeyHold("Human/AttackDefault"))
            {
                self.Fire();
            }
            if (Input.GetKeyDown("Interaction/Interact"))
            {
                self._human.Unmount();
                self.NetworkView.Transfer(Network.MasterClient);
                self._inUse = false;
                self.ResetBarrel();
                return;
            }
        }
        if (self.NetworkView.Owner == Network.MyPlayer && self._inUse)
        {
            if (self.NetworkView.Owner.Character == null || self.NetworkView.Owner.Character.Type != "Human" || self.NetworkView.Owner.Character.MountedTransform != self._humanMount)
            {
                self.NetworkView.Transfer(Network.MasterClient);
                self._inUse = false;
                self.ResetBarrel();
                return;
            }
        }
        if (!self._inUse && self._collidingHuman != null)
        {
            if (Input.GetKeyDown("Interaction/Interact")) 
            {
                if (self.NetworkView.Owner == Network.MyPlayer) 
                {
                    self._inUse = true;
                    self._collidingHuman.MountTransform(self._humanMount, Vector3.Zero, Vector3.Zero);
                    self._human = self._collidingHuman;
                }
                else
                {
                    self.NetworkView.SendMessage(self.NetworkView.Owner, "request");
                }
            }
        }
    }

    function ResetBarrel()
    {
        self._barrel.LocalRotation = Vector3(0, 0, 0);
    }

    function Fire()
    {
        self._cooldownLeft = self.Cooldown;
        self._ammoLeft = self._ammoLeft - 1;
        if (self._human != null)
        {
            Game.SpawnEffect("Boom2", self._barrelEnd.Position, self.MapObject.Rotation, 0.5);
            Game.SpawnProjectileWithOwner("CannonBall", self._barrelEnd.Position, Vector3.Zero, self._barrel.Forward.Normalized * self._ballSpeed, 
            Vector3(0, -20, 0), 2.0, self._human);
        }
    }
}
```
