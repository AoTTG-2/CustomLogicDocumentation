# Wagon

The Wagon component allows Wagon2 to become a functional networked wagon. Do not use this on any other objects.

```csharp
component Wagon
{
    MoveForce = 20.0;
    MaxMoveSpeed = 50.0;
    RotateSpeed = 3.0;
    _inUse = false;
    _riding = false;
    _horse = null;
    _human = null;
    _collidingHuman = null;
    _collidingDrive = false;
    _collidingRide = false;
    _collidingGas = false;
    _rigidbody = null;
    _leftWheel = null;
    _rightWheel = null;
    _leftSitTransform = null;
    _rightSitTransform = null;

    function Init()
    {
        self._horse = self.MapObject.GetTransform("Horse");
        self.MapObject.AddSphereCollider("Region", "Characters", Vector3.Zero, 10.0);
        self._rigidbody = self.MapObject.GetComponent("Rigidbody");
        self._leftWheel = self.MapObject.GetTransform("Carriage/Wheels/LeftWheelPivot");
        self._rightWheel = self.MapObject.GetTransform("Carriage/Wheels/RightWheelPivot");
        self._leftSitTransform = self.MapObject.GetTransform("SitRegionBottomLeft");
        self._rightSitTransform = self.MapObject.GetTransform("SitRegionBottomRight");
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
        }
        elif (newOwner == Network.MyPlayer)
        {
            self._inUse = true;
            human = Network.MyPlayer.Character;
            if (human != null && human.Type == "Human")
            {
                human.MountTransform(self._horse, Vector3(0, 1.95, 0), Vector3.Zero);
                self._human = human;
            }
        }
    }

    function OnCollisionStay(other)
    {
        if (other.Type == "Human" && other.IsMine)
        {
            diff = (other.Position - self.MapObject.Position);
            project = Vector3.Project(diff, self.MapObject.Forward);
            if (project.Magnitude > 3 * self.MapObject.Scale.Z && project.Normalized == self.MapObject.Forward)
            {
                if (!self._inUse && !self._riding)
                {
                    UI.SetLabelForTime("MiddleCenter", "Press " + Input.GetKeyName("Interaction/Interact") + " to drive wagon.", 0.1);
                    self._collidingHuman = other;
                    self._collidingDrive = true;
                }
            }
            elif (project.Magnitude > 4 * self.MapObject.Scale.Z && project.Normalized == self.MapObject.Forward * -1.0)
            {
                if (!self._riding)
                {
                    UI.SetLabelForTime("MiddleCenter", "Press " + Input.GetKeyName("Interaction/Interact") + " to ride wagon.", 0.1);
                    self._collidingHuman = other;
                    self._collidingRide = true;
                }
            }
            else
            {
                if (!self._inUse && !self._riding)
                {
                    UI.SetLabelForTime("MiddleCenter", "Press " + Input.GetKeyName("Interaction/Interact") + " to refill.", 0.1);
                    self._collidingHuman = other;
                    self._collidingGas = true;
                }
            }
        }
    }

    function OnTick()
    {
        self._collidingHuman = null;
        self._collidingDrive = false;
        self._collidingRide = false;
        self._collidingGas = false;

        if (self._leftWheel != null && self._rightWheel != null)
        {
            L = Vector3.Distance(self._leftWheel.Position, self._rightWheel.Position);
            r = self._leftWheel.Scale.Y / 2;

            localVelocity = self.MapObject.Transform.InverseTransformDirection(self._rigidbody.GetVelocity());
            angularVelocity = self._rigidbody.GetAngularVelocity();
            
            v_x = localVelocity.Z;
            omega = angularVelocity.Y;

            leftWheelRotationSpeed = (v_x - (L / 2) * omega) / r;
            rightWheelRotationSpeed = (v_x + (L / 2) * omega) / r;

            leftWheelRotation = leftWheelRotationSpeed * Time.TickTime * Math.Rad2DegConstant * 0.3; # Character moves too fast for irl physics
            rightWheelRotation = rightWheelRotationSpeed * Time.TickTime * Math.Rad2DegConstant * 0.3;

            self._leftWheel.Rotate(Vector3(leftWheelRotation, 0, 0));
            self._rightWheel.Rotate(Vector3(rightWheelRotation, 0, 0));

        }
    }

    function OnFrame()
    {
        if (self.NetworkView.Owner == Network.MyPlayer)
        {
            if (self._inUse)
            {
                if (self._human.HasTargetDirection)
                {
                    self.MapObject.Forward = Vector3.Lerp(self.MapObject.Forward, self._human.TargetDirection, self.RotateSpeed * Time.FrameTime);
                    self._rigidbody.AddForce(self.MapObject.Forward * self.MoveForce);
                    velocity = self._rigidbody.GetVelocity();
                    self._rigidbody.SetVelocity(velocity.Normalized * Math.Min(velocity.Magnitude, self.MaxMoveSpeed));
                }
                else
                {
                    velocity = self._rigidbody.GetVelocity();
                    if (velocity.Magnitude < 1)
                    {
                        self._rigidbody.SetVelocity(Vector3.Up * velocity.Y);
                    }
                    else
                    {
                        self._rigidbody.AddForce(-0.5 * velocity.Normalized * velocity.Magnitude);
                    }
                }
                if (self._rigidbody.GetVelocity().Magnitude > 1)
                {
                    self._human.PlayAnimation("Armature|horse_run");
                }
                else
                {
                    self._human.PlayAnimation("Armature|horse_idle");
                }
                if (Input.GetKeyDown("Interaction/Interact"))
                {
                    self._human.Unmount();
                    self.NetworkView.Transfer(Network.MasterClient);
                    self._inUse = false;
                    return;
                }
                if (self.NetworkView.Owner.Character == null || self.NetworkView.Owner.Character.Type != "Human" || self.NetworkView.Owner.Character.MountedTransform != self._horse)
                {
                    self.NetworkView.Transfer(Network.MasterClient);
                    self._inUse = false;
                    return;
                }
            }
            else
            {
                velocity = self._rigidbody.GetVelocity();
                if (velocity.Magnitude < 1)
                {
                    self._rigidbody.SetVelocity(Vector3.Up * velocity.Y);
                }
                else
                {
                    self._rigidbody.AddForce(-0.5 * velocity.Normalized * velocity.Magnitude);
                }
            }
        }
        if (self._riding)
        {
            if (self._human == null || self._human.MountedMapObject != self.MapObject)
            {
                self._riding = false;
                return;
            }
            if (Input.GetKeyDown("Interaction/Interact"))
            {
                self._human.Unmount();
                self._riding = false;
            }
            else
            {
                self._human.PlayAnimation("Armature|horse_idle");
            }
        }
        if (self._collidingHuman != null)
        {
            if (Input.GetKeyDown("Interaction/Interact"))
            {
                if (self._collidingDrive && !self._inUse)
                {
                    if (self.NetworkView.Owner == Network.MyPlayer) 
                    {
                        self._inUse = true;
                        self._collidingHuman.MountTransform(self._horse, Vector3(0, 1.95, 0), Vector3.Zero);
                        self._human = self._collidingHuman;
                    }
                    else
                    {
                        self.NetworkView.SendMessage(self.NetworkView.Owner, "request");
                    }
                }
                elif (self._collidingGas && !self._inUse)
                {
                    self._collidingHuman.Refill(true);
                }
                elif (self._collidingRide && !self._riding)
                {
                    self._riding = true;
                    self._human = self._collidingHuman;
                    posA = self._leftSitTransform.LocalPosition; # Vector3(-1.0, 1.78, -3.5);
                    posB = self._rightSitTransform.LocalPosition; # Vector3(1.0, 1.78, 1.0);
                    self._human.MountMapObject(self.MapObject, Random.RandomVector3(posA, posB), Vector3(0, 0, 0));
                }
            }
        }
        self.UpdateHorse();
    }

    function UpdateHorse()
    {
        if (self._rigidbody.GetVelocity().Magnitude > 1)
        {
            self._horse.PlayAnimation("horse_Run");
            self.MapObject.GetTransform("RunSound").PlaySound();
            self.MapObject.GetTransform("Dust").ToggleParticle(true);
        }
        else
        {
            self._horse.PlayAnimation("horse_idle0");
            self.MapObject.GetTransform("RunSound").StopSound();
            self.MapObject.GetTransform("Dust").ToggleParticle(false);
        }
    }
}
```
