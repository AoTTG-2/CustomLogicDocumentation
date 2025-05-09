# Thunderspear PVP

The Thunderspear PVP gamemode is a player versus player mode using only thunderspears.

```csharp
class Main
{   
    PointMode = false;
    MaxPoints = 25;
    RespawnDelay = 5.0;
    InfiniteGas = true;
    _hasSpawned = false;
    _dieTimeLeft = 0.0;

    function OnTick()
    {
        if (Game.IsEnding)
        {
            return;
        }
        if (self.PointMode)
        {
            self.UpdatePointMode();
        }
        else
        {
            self.UpdateLastManMode();
        }
    }

    function OnGameStart()
    {
        Game.SetPlaylist("Battle");
        if (self.PointMode)
        {
            Network.MyPlayer.ClearKDR();
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

    function UpdatePointMode()
    {
        self._dieTimeLeft = self._dieTimeLeft - Time.TickTime;
        if (Network.MyPlayer.Status == "Dead" && self._dieTimeLeft <= 0.0)
        {
            Game.SpawnPlayer(Network.MyPlayer, false);
        }
        if (Game.GetMiscSetting("PVP") == 2)
        {
            redKills = 0;
            blueKills = 0;
            for (player in Network.Players)
            {
                if (player.Team == "Red")
                {
                    redKills = redKills + player.Kills;
                }
                elif (player.Team == "Blue")
                {
                    blueKills = blueKills + player.Kills;
                }
            }
            if (Network.IsMasterClient)
            {
                if (redKills >= self.MaxPoints)
                {
                    UI.SetLabelAll("MiddleCenter", "Red team wins!");
                    Game.End(10.0);
                }
                elif (blueKills >= self.MaxPoints)
                {
                    UI.SetLabelAll("MiddleCenter", "Blue team wins!");
                    Game.End(10.0);
                }
            }
            UI.SetLabel("TopCenter", "Red: " + Convert.ToString(redKills) + "   Blue: " + Convert.ToString(blueKills));
        }
        else
        {
            if (Network.IsMasterClient)
            {
                for (player in Network.Players)
                {
                    if (player.Kills >= self.MaxPoints)
                    {
                        UI.SetLabelAll("MiddleCenter", player.Name + " wins!");
                        Game.End(10.0);
                    }
                }
            }
            UI.SetLabel("TopCenter", "Points: " + Convert.ToString(Network.MyPlayer.Kills));
        }
    }

    function UpdateLastManMode()
    {
        humans = Game.Humans.Count;
        if (Network.IsMasterClient)
        {
            if (humans > 1)
            {
                self._hasSpawned = true;
            }
            elif (humans == 1 && self._hasSpawned)
            {
                UI.SetLabelAll("MiddleCenter", Game.Humans.Get(0).Player.Name + " wins!");
                Game.End(10.0);
            }
            elif (humans == 0 && self._hasSpawned)
            {
                UI.SetLabelAll("MiddleCenter", "Nobody wins!");
                Game.End(10.0);
            }
        }
        UI.SetLabel("TopCenter", "Players alive: " + Convert.ToString(humans));
    }
}
```
