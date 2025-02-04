# Expressions

Expressions allow us to combine or modify variables, such as addition, subtraction, etc.

We already looked at one type of expression, which is the **set** expression. This assigns a value to a variable.

```csharp
myFloat = 5.5;
```

We can modify this float variable through addition, subtraction, division, multiplication expressions.

```csharp
myFloat = myFloat + 5.0;
myFloat = 5.0 / 3.0;
myFloat = (myFloat * 2.0) - 3.5;
myFloat += 5.0;
```

Parentheses can be used to specify operation priority as in the third example.

Be careful not to perform operations on incompatible types. This would throw an error:

```csharp
vector = Vector3(0, 0, 0);
myInt = 5;
Game.Print(vector + myInt);
```

You can't add a vector and an int together! Instead, lets convert the int to vector first before adding them.

```csharp
Game.Print(vector + Vector3(myInt, myInt, myInt));
```

This will print out "5, 5, 5".

We can reference other class fields or method calls in our expressions.

```csharp
myString = Network.MyPlayer.Name + " joined at " + Convert.ToString(Time.GameTime);
```

Finally, we can use some symbols to modify bool values. They include the following:

* \== (equals)
* != (not equals)
* || (or)
* && (and)
* ! (not)
* < (less than)
* \>(greater than)
* <= (less than or equal)
* \>= (greater than or equal)

```
myInt = 5;
myBool = myInt == 5; (this returns true)
myBool = !(myInt == 5); (this returns false)
myBool = myInt != 5; (this returns false)
myBool = (myInt == 4 || myInt == 5); (this returns true)
myBool = myInt == 4 && myInt == 5; (this returns false)
myBool = myInt >= 4; (this returns true)
```
