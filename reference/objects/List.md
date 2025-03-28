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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Clear</mark>()
> Clear all list elements
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Get</mark>(<mark style="color:blue;">int</mark> index)
> Get the element at the specified index
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Set</mark>(<mark style="color:blue;">int</mark> index, <mark style="color:blue;">Object</mark> value)
> Set the element at the specified index
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Add</mark>(<mark style="color:blue;">Object</mark> value)
> Add an element to the end of the list
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">InsertAt</mark>(<mark style="color:blue;">int</mark> index, <mark style="color:blue;">Object</mark> value)
> Insert an element at the specified index
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">RemoveAt</mark>(<mark style="color:blue;">int</mark> index)
> Remove the element at the specified index
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Remove</mark>(<mark style="color:blue;">Object</mark> value)
> Remove the first occurrence of the specified element
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">Contains</mark>(<mark style="color:blue;">Object</mark> value)
> Check if the list contains the specified element
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Sort</mark>()
> Sort the list
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SortCustom</mark>(<mark style="color:blue;">UserMethod</mark> method)
> Sort the list using a custom method, expects a method with the signature int method(a,b)
#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">Filter</mark>(<mark style="color:blue;">UserMethod</mark> method)
> Filter the list using a custom method, expects a method with the signature bool method(element)
#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">Map</mark>(<mark style="color:blue;">UserMethod</mark> method)
> Map the list using a custom method, expects a method with the signature object method(element)
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Reduce</mark>(<mark style="color:blue;">UserMethod</mark> method, <mark style="color:blue;">Object</mark> initialValue)
> Reduce the list using a custom method, expects a method with the signature object method(acc, element)
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Randomize</mark>()
> Randomize the list
#### <mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">ToSet</mark>()
> Convert the list to a set

---

