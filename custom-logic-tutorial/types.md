# Types

Variables have different types, such as strings, bools, ints, Human, Titan, etc. Custom logic uses type inferencing, meaning variable types are not explicitly declared but are inferred based on their assignments.

**Primitive types** are the most basic types of variable. They include:

* string ("hello world"). Strings represent text and are declared by enclosing anything with double quotations (" ").&#x20;
* float (5.0). Floats represent decimal numbers and are declared by any number with a decimal point.
* int (5). Ints represent integer numbers and are declared by any number without a decimal.
* bool (true/false). Bools represent true or false and are declared by using the true or false keywords.
* null. Null represents the empty or null value, and can be declared by using the null keyword.

Some examples of each primitive being declared:

```csharp
class Main
{
    MyString = "Hello world";
    MyFloat = 5.0;
    MyInt = 5;
    MyBool = true;
    MyNull = null;
}
```

**Object types** are variable types that are derived from classes. There are also many builtin object types, such as Human, Titan, Vector3, Player. These types are often passed in callback functions.

```csharp
class Main
{
    function OnPlayerSpawn(player, character)
    {
        Game.Print(player.Name);
    }
}
```

In this example, player is of type Player and character is of type Character. As objects, they may have variable fields that can be referenced such as player.Name.

Some object types, such as Vector3, Color, or any object types that derive from custom classes can be created and assigned to a variable. This is called **instantiation.**

```csharp
class Main
{
    function OnPlayerSpawn(player, character)
    {
        newSpawnPosition = Vector3(0.0, 100.0, 0.0);
        character.Position = newSpawnPosition;
    }
}
```

Here we create a new Vector3 by using the Vector3(x, y, z) initializer. We then assign it to newSpawnPosition. Finally, we set the character's position to this Vector3 variable. The effect of this script is that every character will be immediately moved to the (0, 100, 0) position upon spawning.
