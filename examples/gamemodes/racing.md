# Racing

The Racing gamemode starts by removing a start barrier and ends when a player reaches the end region.

{% code fullWidth="false" %}
```csharp
class Main
{   
    Description = "Navigate the obstacle course as quickly as possible. Move towards green checkpoints and avoid the red kill regions.";
    StartDelay = 10.0;
    EndAfterWin = true;
    InfiniteLives = true;
    Lives = 0;
    RespawnDelay = 1.5;
    _started = false;
    _startBarriers = null;
    _dieTimeLeft = 0.0;
    _livesLeft = 0;
    _finished = false;
    _hasSpawned = false;

    function OnGameStart()
    {
        self._startBarriers = Map.FindMapObjectsByTag("RacingStartBarrier");
        self._livesLeft = self.Lives;
        Network.MyPlayer.SetCustomProperty("NoLivesLeft", false);
        Game.SetPlaylist("Racing");
    }

    function FinishRace(human)
    {
        if (!self._finished)
        {
            Game.PrintAll(human.Player.Name + " finished at " + String.FormatFloat(Time.GameTime - self.StartDelay, 2));
            Network.SendMessage(Network.MasterClient, "Finish");
            self._finished = true;
        }
    }

    function OnNetworkMessage(sender, message)
    {
        if (Network.IsMasterClient && message == "Finish" && !Game.IsEnding && self.EndAfterWin)
        {
            UI.SetLabelAll("MiddleCenter", sender.Name + " has won the race!");
            Game.End(10);
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
        if (!self._started)
        {
            Game.SpawnPlayer(Network.MyPlayer, false);
            UI.SetLabel("TopCenter", "Race Starts In: " + String.FormatFloat(self.StartDelay - Time.GameTime, 2));
            if (Time.GameTime > self.StartDelay)
            {
                self._started = true;
                for (barrier in self._startBarriers)
                {
                    barrier.Active = false;
                }
                if (Network.MyPlayer.Status == "Alive")
                {
                    self._hasSpawned = true;
                }
            }
        }
        else
        {
            if (!self.InfiniteLives)
            {
                UI.SetLabel("TopCenter", "Racing Time: " + String.FormatFloat(Time.GameTime - self.StartDelay, 2) + ", Lives: " + Convert.ToString(self._livesLeft));
            }
            else
            {
                UI.SetLabel("TopCenter", "Racing Time: " + String.FormatFloat(Time.GameTime - self.StartDelay, 2));
            }
            self._dieTimeLeft = self._dieTimeLeft - Time.TickTime;
            if (!self._hasSpawned && Network.MyPlayer.Status == "Dead")
            {
                Game.SpawnPlayer(Network.MyPlayer, false);
                self._hasSpawned = true;
            }
            elif (Network.MyPlayer.Status == "Dead" && self._dieTimeLeft <= 0.0)
            {
                if (self._livesLeft > 0 || self.InfiniteLives)
                {
                    Game.SpawnPlayer(Network.MyPlayer, false);
                    self._livesLeft = self._livesLeft - 1;
                }
                else
                {
                    Network.MyPlayer.SetCustomProperty("NoLivesLeft", true);
                }
            }
            if (Network.IsMasterClient && !Game.IsEnding)
            {
                anyPlayerAlive = false;
                anyPlayerSpawned = false;
                for (player in Network.Players)
                {
                    if (player.Status != "Spectating")
                    {
                        anyPlayerSpawned = true;
                        noLivesLeft = player.GetCustomProperty("NoLivesLeft");
                        if (player.Status == "Alive" || (noLivesLeft != null && !noLivesLeft))
                        {
                            anyPlayerAlive = true;
                        }
                    }
                }
                if (anyPlayerSpawned && !anyPlayerAlive)
                {
                    UI.SetLabelAll("MiddleCenter", "All players have no lives left.");
                    Game.End(10);
                }
            }
        }
    }
}

```
{% endcode %}
