# Dummy

The Dummy component allows Dummy2 to become a functional networked dummy titan. Do not use this on any other objects.

```csharp
component Dummy
{
    ResetCount = 0;
    ResetDelay = 5.0;
    _state = "Alive";
    _currentResetTime = 0.0;

    function Init()
    {
        self.MapObject.Transform.PlayAnimation("Armature|dummy_idle");
        self.MapObject.AddSphereCollider("Region", "Hitboxes", Vector3(0, 12.4, -3.7), 1.0);
    }

    function OnNetworkMessage(sender, message)
    {
        if (message == "hit")
        {
            if (self._state == "Alive")
            {
                self.MapObject.Transform.PlayAnimation("Armature|dummy_fall");
                self.MapObject.GetTransform("FallSound").PlaySound();
            }
            self._currentResetTime = self.ResetDelay;
            self._state = "Dead";
        }
    }

    function OnTick()
    {
        self._currentResetTime = self._currentResetTime - Time.TickTime;
        if (self._state == "Dead")
        {
            if (self._currentResetTime <= 0 && self.ResetCount > 0)
            {
                self.ResetCount = self.ResetCount - 1;
                self._state = "Rise";
                self.MapObject.Transform.PlayAnimation("Armature|dummy_rise");
                self.MapObject.GetTransform("RiseSound").PlaySound();
                self._currentResetTime = 1.0;
            }
        }
        elif (self._state == "Rise")
        {
            if (self._currentResetTime <= 0)
            {
                self._state = "Alive";
                self.MapObject.Transform.PlayAnimation("Armature|dummy_idle");
            }
        }
    }

    function OnGetHit(character, name, damage, type)
    {
        if (self._state == "Alive")
        {
            self.NetworkView.SendMessageAll("hit");
        }
    }
}
```
