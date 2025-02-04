# Classes

Classes allow you create modular pieces of code, which can be useful for separating custom logic into manageable pieces. In the previous section we explored the Main class, which is a special class that is always initialized and run upon game start. Besides Main, there are several kinds of classes: Normal classes, components, extensions, and cutscenes. For now we will look at the normal class.

```csharp
class Main
{
    function Init()
    {
        numberPrinter = NumberPrinter();
        numberPrinter.Print(5);
    }
}

class NumberPrinter
{
    function Init()
    {
        Game.Print("Init");
    }
    
    function Print(num)
    {
        Game.Print(Convert.ToString(num));
    }
}
```

`function Init()` is called in every class upon creation.

`class NumberPrinter` declares a new class NumberPrinter, similar to the way we declared the Main class. Since this is a normal class it does not have access to the callback functions that Main has, except for Init().&#x20;

`numberPrinter = NumberPrinter()` creates an instance of the NumberPrinter class and stores it in the numberPrinter variable.&#x20;

`numberPrinter.Print(5)` calls the Print function on our instance variable. The output of this program is "Init" followed by "5".

Like Main, custom classes can contain their own instance variables and functions.\
