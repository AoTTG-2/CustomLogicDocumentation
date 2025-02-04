# KillRegion

The KillRegion component kills characters that enter the region.

```csharp
component KillRegion
{
    Team = "None";
    KillHumans = true;
    KillTitans = true;
    KillShifters = true;
    KillMessage = "Server";

    function OnCollisionEnter(other)
    {
        if (other.IsCharacter && other.IsMine)
        {
            if (other.Type == "Human" && !self.KillHumans)
            {
                return;
            }
            if (other.Type == "Titan" && !self.KillTitans)
            {
                return;
            }
            if (other.Type == "Shifter" && !self.KillShifters)
            {
                return;
            }
            if (other.Team != self.Team && self.Team != "None")
            {
                return;
            }
            other.GetKilled(self.KillMessage);
        }
    }
}
```
