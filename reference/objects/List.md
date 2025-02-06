# List
Inherits from object
## Initialization
```csharp
example = List()
example = List((CustomLogicSetBuiltin))
```
## Fields
|<div style="width:30%">Field</div>|<div style="width:10%">Type</div>|<div style="width:10%">Readonly</div>|<div style="width:50%">Description</div>|
|---|---|---|---|
|Count|int|True|The number of elements in the list|
## Methods
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|Clear()|none|Clear all list elements|
|Get(index : int)|Object|Get the element at the specified index|
|Set(index : int,<br/>value : Object)|none|Set the element at the specified index|
|Add(value : Object)|none|Add an element to the end of the list|
|InsertAt(index : int,<br/>value : Object)|none|Insert an element at the specified index|
|RemoveAt(index : int)|none|Remove the element at the specified index|
|Remove(value : Object)|none|Remove the first occurrence of the specified element|
|Contains(value : Object)|bool|Check if the list contains the specified element|
|Sort()|none|Sort the list|
|SortCustom(method : UserMethod)|none|Sort the list using a custom method, expects a method with the signature int method(a,b)|
|Filter(method : UserMethod)|[List](../objects/List.md)|Filter the list using a custom method, expects a method with the signature bool method(element)|
|Map(method : UserMethod)|[List](../objects/List.md)|Map the list using a custom method, expects a method with the signature object method(element)|
|Reduce(method : UserMethod,<br/>initialValue : Object)|Object|Reduce the list using a custom method, expects a method with the signature object method(acc, element)|
|Randomize()|none|Randomize the list|
|ToSet()|[Set](../objects/Set.md)|Convert the list to a set|
