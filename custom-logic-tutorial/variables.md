# Variables

Variables are a way of storing data, and can be of different types. These types include primitives (string, bool, int, float, null), builtin object types such as Human or Titan, and any custom classes that you define.

We modify our previous example by using `message = "Hello world"`. This stores the "Hello world" string in the message variable, which can then be passed to Game.Print.&#x20;

```csharp
class Main
{
    function OnGameStart()
    {
        message = "Hello world";
        Game.Print(message);
    }
}
```

In this case, message is a **local** variable. This means that it is only usable in the function it was declared in. If we want to use the variable elsewhere, such as in a different function or class, we will need to declare an **instance** variable.&#x20;

```csharp
class Main
{
    Message = "";

    function OnGameStart()
    {
        self.Message = "Hello world";
        Game.Print(self.Message);
    }
}
```

Notice that instance variables within the class are referenced by using the self keyword. If we were to reference this variable outside of Main, we would use Main.Message.
