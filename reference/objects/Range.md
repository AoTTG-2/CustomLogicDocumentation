# Range
## Initialization
```csharp
example = Range((Object[]))
```
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Count|int|True|The number of elements in the list|
## Methods
|Function|Returns|Description|
|---|---|---|
|Clear()|none|Clear all list elements|
|Get(<i>index</i> : int)|Object|Get the element at the specified index|
|Set(<br/><i>index</i> : int,<br/><i>value</i> : Object<br/>)|none|Set the element at the specified index|
|Add(<i>value</i> : Object)|none|Add an element to the end of the list|
|InsertAt(<br/><i>index</i> : int,<br/><i>value</i> : Object<br/>)|none|Insert an element at the specified index|
|RemoveAt(<i>index</i> : int)|none|Remove the element at the specified index|
|Remove(<i>value</i> : Object)|none|Remove the first occurrence of the specified element|
|Contains(<i>value</i> : Object)|bool|Check if the list contains the specified element|
|Sort()|none|Sort the list|
|SortCustom(<i>method</i> : UserMethod)|none|Sort the list using a custom method, expects a method with the signature int method(a,b)|
|Filter(<i>method</i> : UserMethod)|[List](../objects/List.md)|Filter the list using a custom method, expects a method with the signature bool method(element)|
|Map(<i>method</i> : UserMethod)|[List](../objects/List.md)|Map the list using a custom method, expects a method with the signature object method(element)|
|Reduce(<br/><i>method</i> : UserMethod,<br/><i>initialValue</i> : Object<br/>)|Object|Reduce the list using a custom method, expects a method with the signature object method(acc, element)|
|Randomize()|none|Randomize the list|
|ToSet()|[Set](../objects/Set.md)|Convert the list to a set|
