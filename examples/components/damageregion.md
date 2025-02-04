# DamageRegion

The DamageRegion component damages characters that enter the region.

```csharp
component DamageRegion
{
    Damage = 1;
    Team = "None";
    DamageHumans = true;
    DamageTitans = true;
    DamageShifters = true;
    KillMessage = "Server";

    function OnCollisionEnter(other)
    {
        if (other.IsCharacter && other.IsMine)
        {
            if (other.Type == "Human" && !self.DamageHumans)
            {
                return;
            }
            if (other.Type == "Titan" && !self.DamageTitans)
            {
                return;
            }
            if (other.Type == "Shifter" && !self.DamageShifters)
            {
                return;
            }
            if (other.Team != self.Team && self.Team != "None")
            {
                return;
            }
            other.GetDamaged(self.KillMessage, self.Damage);
        }
    }
}
```
