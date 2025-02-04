# Conditionals

Conditionals allow us to execute blocks of code based on certain boolean conditions. They include if, else, and elif.

Lets take a look at the basic if conditional, which will execute the block if the condition in parentheses evaluates to true.

```csharp
function OnGameStart()
{
    numPlayers = Network.Players.Count;
    if (numPlayers > 8)
    {
        Game.Print("Too many players!");
    }
}
```

We can also chain conditionals together by using elif and else. The second elif (else if) block will execute only if its conditional passes **and** the first conditional failed. The third else statement will always execute as long as the first two conditionals failed.

```csharp
function OnGameStart()
{
    numPlayers = Network.Players.Count;
    if (numPlayers > 8)
    {
        Game.Print("Too many players!");
    }
    elif (numPlayers > 4)
    {
        Game.Print("Just the right number of players.");
    }
    else
    {
        Game.Print("Too few players!");
    }
}
```

Conditionals can also use expressions in their check statement.

```
if ((numPlayers * 2) > 8 || numPlayers <= 4 * 3)
```
