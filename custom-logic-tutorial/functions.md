# Functions

Functions are pieces of executable code within classes. There are two types of functions: custom and callback. Custom functions are only called when explicitly used in the script, while callback functions are called based on certain conditions. Both however are declared the same way.

Let's first create a helper function that spawns some titans at certain locations.

```csharp
class Main
{
    function OnGameStart()
    {
        self.SpawnTitans(8);
    }
    
    function SpawnTitans(num)
    {
        location1 = Vector3(-50, 0, 0);
        location2 = Vector3(50, 0, 0);
        Game.SpawnTitansAt("Default", num, location1);
        Game.SpawnTitansAt("Default", num, location2);
    }
}
```

OnGameStart is a callback function that is called once upon the game round starting. SpawnTitans is a custom function that is unused until we call it in OnGameStart. Here we spawn 8 titans each at the positions (-50, 0, 0) and (50, 0, 0).

Notice the self that precedes the function call. This is used to reference anything that is defined in the current class, including instance variables and functions. On the other hand, we reference the Game class in order to call its SpawnTitansAt function.

When declaring the SpawnTitans function, we included a **parameter** num. Parameters allow us to pass values when calling the function, which can then be used as a local variable within the function.

Functions can also return values.

```csharp
class Main
{
    function OnCharacterDie(victim, killer, name)
    {
        if (killer != null)
        {
            damage = self.CalculateDamage(killer.Velocity);
            Game.Print(name + " dealt " + Convert.ToString(damage));
        }
    }
    
    function CalculateDamage(velocity)
    {
        damage = velocity.Magnitude * 10.0;
        return damage;
    }
}
```

Here, OnCharacterDie is a callback function that is called whenever a character dies. The CalculateDamage function returns a float value that can then be used in OnCharacterDie to print out the damage dealt.
