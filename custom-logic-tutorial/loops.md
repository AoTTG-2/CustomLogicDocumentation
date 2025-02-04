# Loops

Loops allow us to execute blocks of code continuously. There are two kinds of loops: while, and for.

Lets take a look at the while loop, which will execute the block repeatedly until the conditional fails.

```csharp
i = 0;
while (i < 10)
{
    Game.Print(Convert.ToString(i));
    i = i + 1;
}
```

This will print out 0 to 9, since once i reaches 10 the loop will break.

For loops allow us to iterate over collections such as lists and ranges.

```csharp
for (player in Network.Players)
{
    Game.Print(player.Name);
}
```

Here, Network.Players returns a List of players which is an **iterable,** meaning it can be read in sequence. This for loop will print out each player's name.

The Range() class allows us to create convenient iterables of integers to loop over. This is useful if you want to quickly iterate over a range of numbers for example.

```csharp
for (i in Range(0, 10, 1))
{
    Game.SpawnTitans("Default", i);
}
```

Range takes 3 ints: Start, End, and Step. Start is the first number the range begins at, End is the last number (exclusive), and Step is how much the variable will increment each loop. In this case, i begins at 0, increases by 1 at each loop, and breaks once it reaches 10.
