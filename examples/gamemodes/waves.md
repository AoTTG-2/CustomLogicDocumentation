# Waves

The Waves gamemode spawns an increasing number of titans for a certain number of waves.

```
class Main
{   
    Description = "Survive multiple waves of titans.";
    StartTitans = 3;
    AddTitansPerWave = 1;
    MaxWaves = 20;
    RespawnOnWave = true;
    GradualSpawn = true;
    GradualSpawnTooltip = "Spawn new titans gradually over time. Helpful for reducing lag.";
    _currentWave = 0;
    _hasSpawned = false;

    function OnGameStart()
    {
        if (Network.IsMasterClient)
        {
            self.NextWave();
        }
    }

    function OnCharacterSpawn(character)
    {
        if (character.IsMine && character.Type == "Titan")
        {
            character.DetectRange = 2000;
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
                self.NextWave();
            }
            if (humans == 0 && playerShifters == 0 && self._hasSpawned)
            {
                UI.SetLabelAll("MiddleCenter", "Humanity failed!");
                Game.End(10.0);
                return;
            }
            UI.SetLabelAll("TopCenter", "Titans Left: " + Convert.ToString(titans) + "  " + "Wave: " + Convert.ToString(self._currentWave));
        }
    }

    function NextWave()
    {
        self._currentWave = self._currentWave + 1;
        if (self._currentWave > self.MaxWaves)
        {
            UI.SetLabelAll("MiddleCenter", "All waves cleared, humanity wins!");
            Game.End(10.0);
            return;
        }
        amount = self.AddTitansPerWave * (self._currentWave - 1) + self.StartTitans;
        if (self.GradualSpawn)
        {
            Game.SpawnTitansAsync("Default", amount);
        }
        else
        {
            Game.SpawnTitans("Default", amount);
        }
        if (self.RespawnOnWave)
        {
            Game.SpawnPlayerAll(false);
        }
    }
}

```
