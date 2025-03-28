# List
Inherits from object
## Initialization
```csharp
example = List()
example = List((CustomLogicSetBuiltin))
```
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Count|int|True|The number of elements in the list|
## Methods
#### void <span style="color":#dcdcaa>Clear<span>()
Clear all list elements
#### Object <span style="color":#dcdcaa>Get<span>(int <span style="color":#9cdcfe>index<span>)
Get the element at the specified index
#### void <span style="color":#dcdcaa>Set<span>(int <span style="color":#9cdcfe>index<span>, Object <span style="color":#9cdcfe>value<span>)
Set the element at the specified index
#### void <span style="color":#dcdcaa>Add<span>(Object <span style="color":#9cdcfe>value<span>)
Add an element to the end of the list
#### void <span style="color":#dcdcaa>InsertAt<span>(int <span style="color":#9cdcfe>index<span>, Object <span style="color":#9cdcfe>value<span>)
Insert an element at the specified index
#### void <span style="color":#dcdcaa>RemoveAt<span>(int <span style="color":#9cdcfe>index<span>)
Remove the element at the specified index
#### void <span style="color":#dcdcaa>Remove<span>(Object <span style="color":#9cdcfe>value<span>)
Remove the first occurrence of the specified element
#### bool <span style="color":#dcdcaa>Contains<span>(Object <span style="color":#9cdcfe>value<span>)
Check if the list contains the specified element
#### void <span style="color":#dcdcaa>Sort<span>()
Sort the list
#### void <span style="color":#dcdcaa>SortCustom<span>(UserMethod <span style="color":#9cdcfe>method<span>)
Sort the list using a custom method, expects a method with the signature int method(a,b)
#### [List](../objects/List.md) <span style="color":#dcdcaa>Filter<span>(UserMethod <span style="color":#9cdcfe>method<span>)
Filter the list using a custom method, expects a method with the signature bool method(element)
#### [List](../objects/List.md) <span style="color":#dcdcaa>Map<span>(UserMethod <span style="color":#9cdcfe>method<span>)
Map the list using a custom method, expects a method with the signature object method(element)
#### Object <span style="color":#dcdcaa>Reduce<span>(UserMethod <span style="color":#9cdcfe>method<span>, Object <span style="color":#9cdcfe>initialValue<span>)
Reduce the list using a custom method, expects a method with the signature object method(acc, element)
#### void <span style="color":#dcdcaa>Randomize<span>()
Randomize the list
#### [Set](../objects/Set.md) <span style="color":#dcdcaa>ToSet<span>()
Convert the list to a set

---

