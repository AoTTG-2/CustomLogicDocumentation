# Static Classes

You may have noticed that some classes, such as Game or Convert can be referenced directly without first creating an instance. These are known as **static classes** - meaning there is only one instance that can be globally accessed from anywhere in the script. Many common functions, such as spawning titans and performing math operations, will be found in these static classes.

```csharp
class Main
{
    function OnGameStart()
    {
        numTitans = Math.Pow(2, 5);
        Game.SpawnTitans("Default", numTitans);
    }
}
```

Main is also a static class, and can be referenced from anywhere just like Math or Game.

```csharp
class TitanSpawner
{
    function Spawn()
    {
        num = Main.TitansPerWave;
        Game.SpawnTitans("Default", num);
    }
}
```
