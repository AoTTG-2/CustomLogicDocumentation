# Survive

The Survive gamemode spawns a set number of titans and ends when either all titans or all humans are dead.

```csharp
class Main
{   
    Description = "Survive a single round of titans.";
    Titans = 15;
    _hasSpawned = false;

    function OnGameStart()
    {
        if (Network.IsMasterClient)
        {
            Game.SpawnTitans("Default", self.Titans);
        }
    }

    function OnTick()
    {
        if (Network.IsMasterClient && !Game.IsEnding)
        {
            titans = Game.Titans.Count;
            humans = Game.Humans.Count;
            playerShifters = Game.PlayerShifters.Count;
            if (humans > 0 || playerShifters > 0)
            {
                self._hasSpawned = true;
            }
            if (titans == 0)
            {
                UI.SetLabelAll("MiddleCenter", "Humanity wins!");
                Game.End(10.0);
                return;
            }
            if (humans == 0 && playerShifters == 0 && self._hasSpawned)
            {
                UI.SetLabelAll("MiddleCenter", "Humanity failed!");
                Game.End(10.0);
                return;
            }
            UI.SetLabelAll("TopCenter", "Titans Left: " + Convert.ToString(titans));
        }
    }
}
```
