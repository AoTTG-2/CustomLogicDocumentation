# Titan Explode

The Titan Explode gamemode has titans explode and kill all players in radius upon death.

```csharp
class Main
{   
    Description = "Titans will explode on death.";
    ExplodeRadius = 30.0;
    MaxTitans = 10;
    TitanSpawnEvery = 3.0;
    _spawnTimeLeft = 0.0;
    _hasSpawned = false;

    function OnGameStart()
    {
        if (Network.IsMasterClient)
        {
            Game.SpawnTitans("Default", self.MaxTitans);
        }
    }

    function OnCharacterDie(victim, killer, killerName)
    {
        if (victim.Type == "Titan" && victim.IsMine)
        {
            if (victim.IsCrawler)
            {
                self.Explode(victim.NapePosition, 2.0);
            }
            else
            {
                self.Explode(victim.NapePosition, 1.0);
            }
        }
    }

    coroutine Explode(position, time)
    {
        wait time;
        Game.SpawnEffect("ThunderspearExplode", position, Vector3.Zero, self.ExplodeRadius * 2.0, Color(255, 255, 255, 255));
        for (human in Game.Humans)
        {
            if (Vector3.Distance(human.Position, position) < self.ExplodeRadius)
            {
                human.GetKilled("Explosion");
            }
        }
    }

    function OnTick()
    {
        if (Network.IsMasterClient && !Game.IsEnding)
        {
            humans = Game.Humans.Count;
            playerShifters = Game.PlayerShifters.Count;
            titans = Game.Titans.Count;
            if (humans > 0 || playerShifters > 0)
            {
                self._hasSpawned = true;
            }
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
