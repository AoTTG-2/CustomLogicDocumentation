# Your first script

Now that you know how to load custom logic into a map, let's create our first custom logic script. This script will be simple - it will start the game and print "Hello world" to the chat window.

**The Main class**

The core of every custom logic script is the Main class. This class is responsible for most of the game mode logic, and receives important event callbacks.

```csharp
class Main
{
    function OnGameStart()
    {
        Game.Print("Hello world");
    }
}
```

Here, `class Main` means we are declaring a new class named Main. The class named Main is a special class that is always running and always receives event updates.&#x20;

`function OnGameStart()` means we are declaring a new function named OnGameStart that takes no parameters. OnGameStart is a special function known as an **event callback.** This means that it gets called by the interpreter under certain circumstances. In this case, OnGameStart is called once every time the game begins.

`Game.Print("Hello world");` means we are calling the Game.Print function, which prints out a message to the chat window.

Notice that curly braces are used to enclose classes and functions, while semicolons are used to end statements.
