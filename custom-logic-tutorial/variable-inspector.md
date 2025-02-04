# Variable Inspector

Instance variables in the Main class, as well as components, are by default modifiable by the game host. This means that they show up in the "Mode" panel of the game creation window, allowing for hosts to set custom variables for each game mode. Likewise, variables declared in components are visible in the map editor inspector to allow customization across different map objects.

To disable this behavior and make the variable private, precede it with an underscore. This will hide the variable from the inspector.

```csharp
class Main
{
    TitansPerWave = 3;
    _privateVariable = false;
}
```

TitansPerWave will be visible and modifiable by the game host, while \_privateVariable will not be visible.



The **Description** variable, when set to a string, is also shown as a message beneath the Mode panel. This is useful for listing any details you want players to know about the game mode.

```csharp
class Main
{
    Description = "This is a PVP game mode with infinite respawns.";
}
```



The **Tooltip** suffix on any Main variable will give additional gamemode information to the player about certain settings. Tooltips are any variable that ends with "Tooltip". For example, if you have a variable called TitansPerWave, you can add a string field TitansPerWaveTooltip and it will show up as a hint to that setting.

```csharp
class Main
{
    TitansPerWave = 5;
    TitansPerWaveTooltip = "How many titans to spawn per wave.";
}
```



The **Dropbox** suffix on any Main variable will convert that variable into a dropbox with the given comma separated options. For example, if you have a variable called TitanSize, you can add a string field TitanSizeDropbox with comma separated options that will be applied to the TitanSize variable. The initial value of TitanSize will be the default value of the dropbox.&#x20;

**Note that dropboxes only support string variables.**

```csharp
class Main
{
    TitanSize = "Small";
    TitanSizeDropbox = "Small, Medium, Large";
    # Titan Size will now be either "Small", "Medium", or "Large" depending on
    what the user chooses #
}
```
