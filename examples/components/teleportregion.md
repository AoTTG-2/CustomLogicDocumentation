# TeleportRegion

The TeleportRegion component teleports characters who enter the region to another position.

```csharp
component TeleportRegion
{
    RelativePosition = false;
    Position = Vector3(0, 0, 0);
    TeleportHumans = true;
    TeleportTitans = true;
    TeleportShifters = true;

    function Init()
    {
        if (self.RelativePosition)
        {
            self.Position = self.MapObject.Position + self.Position;
        }
    }

    function OnCollisionEnter(other)
    {
        if (other.IsCharacter && other.IsMine)
        {
            if (other.Type == "Human" && !self.TeleportHumans)
            {
                return;
            }
            if (other.Type == "Titan" && !self.TeleportTitans)
            {
                return;
            }
            if (other.Type == "Shifter" && !self.TeleportShifters)
            {
                return;
            }
            other.Position = self.Position;
        }
    }
}
```
