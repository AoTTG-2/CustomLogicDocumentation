# Commenting

Comments allow us to describe code to others reading the custom logic file without interfering with the logic. To make a comment, use the '#' character. Any line starting with '#' will be ignored by the interpreter. You can also use '/\*' and '\*/' to create block comments.

Example:

```csharp
class Main
{
    # this function is called everytime the game starts
    function OnGameStart()
    {
        # spawn some titans
        Game.SpawnTitans("Default", 5);
        
        /* 
           this is a comment block
           that takes up multiple lines
        */
        return;
    }

```
