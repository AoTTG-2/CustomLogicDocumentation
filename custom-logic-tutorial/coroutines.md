# Coroutines

Coroutines are like functions except run in the background, while normal functions will interrupt the game until the function is completed. Coroutines can make use of the "wait" keyword in order to pause the function without blocking the game.

Below is an example of a coroutine that runs a cutscene. The wait calls allow the function to pause in the background without interrupting the main execution. To call coroutines you can call them just like any other function.

```csharp
coroutine Start()
{
    spawn = Map.FindMapObjectByName("AnnieSpawnPoint");
    startPosition = Vector3(-85, 40, 132);
    startRotation = Vector3(2, 12.4, 0);
    velocity = Vector3.GetRotationDirection(startRotation, Vector3.Back).Normalized * 5.0;
    Cutscene.SetCameraPosition(startPosition);
    Cutscene.SetCameraRotation(startRotation);
    Cutscene.SetCameraVelocity(velocity);
    Cutscene.ShowDialogue("Levi1", "Levi", "Defeat the female titan before she escapes the forest!");
    wait 1.0;
    if (Network.IsMasterClient)
    {
        annie = Game.SpawnShifterAt("Annie", spawn.Position);
        annie.Rotation = Vector3(0, 180, 0);
    }
    wait 4.0;
}
```
