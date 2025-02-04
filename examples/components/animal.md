# Animal

Used to give some animal map objects some life. Don't attach to other objects.

```csharp
component Animal
{
    Wanders = true;
    WanderRadius = 50.0;
    WanderSpeed = 5.0;
    WalkAnimation = "";
    IdleAnimations = "";
    ActionAnimations = "";
    ActionSounds = "";
    _stateTimeLeft = 0.0;
    _idleAnimations = List();
    _actionAnimations = List();
    _actionSounds = List();
    _transform = null;
    _originalPosition = null;
    _state = "Idle";
    _targetRotation = null;
    _hasAction = false;

    function Init()
    {
        for (anim in String.Split(self.IdleAnimations, "/"))
        {
            if (anim != "")
            {
                self._idleAnimations.Add(anim);
            }
        }
        for (anim in String.Split(self.ActionAnimations, "/"))
        {
            if (anim != "")
            {
                self._actionAnimations.Add(anim);
            }
        }
        for (anim in String.Split(self.ActionSounds, "/"))
        {
            if (anim != "")
            {
                self._actionSounds.Add(anim);
            }
        }
        self._transform = self.MapObject.Transform;
        self._originalPosition = self._transform.Position;
        self._hasAction = self._actionAnimations.Count > 0;
        self._rigidbody = self.MapObject.GetComponent("Rigidbody");
        self.Idle();
    }

    function OnFrame()
    {  
        self._stateTimeLeft = self._stateTimeLeft - Time.FrameTime;
        if (self._state == "Wander")
        {
            if (Vector3.Distance(self._originalPosition, self._transform.Position) > self.WanderRadius)
            {
                self.Idle();            
            }
            else
            {
                if (self._targetRotation != Vector3.Zero)
                {
                    self.MapObject.Forward = Vector3.Lerp(self.MapObject.Forward, self._targetRotation, 5.0 * Time.FrameTime);
                }
                self._rigidbody.SetVelocity(self.MapObject.Forward * self.WanderSpeed);
            }
        }
        elif (self._state == "Returning")
        {
            if (self._targetRotation != Vector3.Zero)
            {
                self.MapObject.Forward = Vector3.Lerp(self.MapObject.Forward, self._targetRotation, 5.0 * Time.FrameTime);
            }
            self._rigidbody.SetVelocity(self.MapObject.Forward * self.WanderSpeed);
        }
        else
        {
            self._rigidbody.SetVelocity(Vector3.Up * self._rigidbody.GetVelocity().Y);
        }
        if (self._stateTimeLeft <= 0.0)
        {
            if (self._state == "Idle")
            {
                if (self._hasAction && Random.RandomFloat(0.0, 1.0) < 0.7)
                {
                    self.Action();
                }
                else
                {
                    self.Wander();
                }
            }
            else
            {
                self.Idle();
            }
        }
    }

    function Idle()
    {
        self._state = "Idle";
        anim = self._idleAnimations.Get(Random.RandomInt(0, self._idleAnimations.Count));
        self._transform.PlayAnimation(anim, 0.2);
        self._stateTimeLeft = Random.RandomFloat(4.0, 8.0);
    }

    function Action()
    {
        self._state = "Action";
        index = Random.RandomInt(0, self._actionAnimations.Count);
        anim = self._actionAnimations.Get(index);
        self._transform.PlayAnimation(anim, 0.2);
        self._stateTimeLeft = self._transform.GetAnimationLength(anim) + 0.2;
        if (self._actionSounds.Count > index)
        {
            sound = self._actionSounds.Get(index);
            if (sound != "None")
            {
                self._transform.GetTransform(sound).PlaySound();
            }
        }
    }

    function Wander()
    {
        self._state = "Wander";
        self._transform.PlayAnimation(self.WalkAnimation, 0.2);
        self._stateTimeLeft = Random.RandomFloat(3.0, 6.0);
        if (Vector3.Distance(self._transform.Position, self._originalPosition) > self.WanderRadius * 0.7)
        {
            x = self._originalPosition.X - self._transform.Position.X;
            z = self._originalPosition.Z - self._transform.Position.Z;
            self._targetRotation = Vector3(x, 0, z).Normalized;
            self._state = "Returning";
        }
        else
        {
            self._targetRotation = Vector3(Random.RandomFloat(-1.0, 1.0), 0, Random.RandomFloat(-1.0, 1.0)).Normalized;
        }
    }
}
```
