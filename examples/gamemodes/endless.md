# Endless

The Endless gamemode never ends, and continuously respawns titans and players.

```csharp
class Main
{   
    Description = "Endless respawn, endless titans.";
    MaxTitans = 10;
    TitanSpawnEvery = 3.0;
    RespawnDelay = 5.0;
    InfiniteGas = false;
    _spawnTimeLeft = 0.0;
    _dieTimeLeft = 0.0;

    function OnGameStart()
    {
        if (Network.IsMasterClient)
        {
            Game.SpawnTitans("Default", self.MaxTitans);
        }
    }

    function OnCharacterSpawn(character)
    {
        if (character.IsMainCharacter && character.Type == "Human" && self.InfiniteGas)
        {
            character.MaxGas = 100000;
            character.CurrentGas = 100000;
        }
    }

    function OnCharacterDie(victim, killer, killerName)
    {
        if (victim.IsMainCharacter)
        {
            self._dieTimeLeft = self.RespawnDelay;
        }
    }

    function OnTick()
    {
        self._dieTimeLeft = self._dieTimeLeft - Time.TickTime;
        if (Network.MyPlayer.Status == "Dead" && self._dieTimeLeft <= 0.0)
        {
            Game.SpawnPlayer(Network.MyPlayer, false);
        }
        if (Network.IsMasterClient)
        {
            titans = Game.Titans.Count;
            if (titans < self.MaxTitans)
            {
                self._spawnTimeLeft = self._spawnTimeLeft - Time.TickTime;
                if (self._spawnTimeLeft <= 0.0)
                {
                    Game.SpawnTitans("Default", 1);
                    self._spawnTimeLeft = self.TitanSpawnEvery;
                }
            }
            else
            {
                self._spawnTimeLeft = self.TitanSpawnEvery;
            }
            UI.SetLabelAll("TopCenter", "Titans Left: " + Convert.ToString(titans));
        }
    }
}
```
