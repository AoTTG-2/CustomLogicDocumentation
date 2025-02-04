# Extensions

Extensions are a way of creating your own static classes, like Game or Convert. This is useful for creating utility functions that can be used globally.

```csharp
class Main
{
    function OnPlayerJoin(player)
    {
        PrettyPrint.PrintJoin(player.Name);
    }
    
    function OnPlayerLeave(player)
    {
        PrettyPrint.PrintLeave(player.Name);
    }
}

extension PrettyPrint
{
    function PrintJoin(name)
    {
        timestamp = self.GetTimestamp(time.GameTime);
        Game.Print(timestamp + " has joined the room.");
    }
    
    function PrintLeave(name)
    {
        timestamp = self.GetTimestamp(time.GameTime);
        Game.Print(timestamp + " has left the room.");
    }
    
    function GetTimestamp(time)
    {
        time = String.FormatFloat(time, 2);
        return "[" + time + "]";
    }
}
```
