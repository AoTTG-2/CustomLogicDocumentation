# Cutscenes

Cutscenes are a type of class that can be conveniently referenced using the Cutscene static class.

Cutscene classes must contain a coroutine "Start", which will be called upon calling Cutscene.Start(CutsceneClassName: string, full: bool).

```csharp
function OnGameStart()
{
    Game.SetPlaylist("Boss");
    Cutscene.Start("MainCutscene", true);
}

cutscene MainCutscene
{
    coroutine Start()
    {
        spawn = Map.FindMapObjectByName("AnnieSpawnPoint");
        startPosition = Vector3(-85, 40, 132);
        startRotation = Vector3(2, 12.4, 0);
        velocity = Vector3.GetRotationDirection(startRotation, Vector3.Back).Normalized * 5.0;
        Camera.SetPosition(startPosition);
	Camera.SetRotation(startRotation);
	Camera.SetVelocity(velocity);
        Cutscene.ShowDialogue("Levi1", "Levi", "Defeat the female titan before she escapes the forest!");
        wait 1.0;
        if (Network.IsMasterClient)
        {
            annie = Game.SpawnShifterAt("Annie", spawn.Position);
            annie.Rotation = Vector3(0, 180, 0);
        }
        wait 4.0;
    }
}
```
