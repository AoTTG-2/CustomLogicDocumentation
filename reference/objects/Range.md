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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Clear</mark>()
Clear all list elements
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Get</mark>(<mark style="color:blue;">int</mark> <mark style="color:yellow;">index</mark>)
Get the element at the specified index
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Set</mark>(<mark style="color:blue;">int</mark> <mark style="color:yellow;">index</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Set the element at the specified index
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Add</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Add an element to the end of the list
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">InsertAt</mark>(<mark style="color:blue;">int</mark> <mark style="color:yellow;">index</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Insert an element at the specified index
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">RemoveAt</mark>(<mark style="color:blue;">int</mark> <mark style="color:yellow;">index</mark>)
Remove the element at the specified index
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Remove</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Remove the first occurrence of the specified element
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">Contains</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Check if the list contains the specified element
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Sort</mark>()
Sort the list
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SortCustom</mark>(<mark style="color:blue;">UserMethod</mark> <mark style="color:yellow;">method</mark>)
Sort the list using a custom method, expects a method with the signature int method(a,b)
#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">Filter</mark>(<mark style="color:blue;">UserMethod</mark> <mark style="color:yellow;">method</mark>)
Filter the list using a custom method, expects a method with the signature bool method(element)
#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">Map</mark>(<mark style="color:blue;">UserMethod</mark> <mark style="color:yellow;">method</mark>)
Map the list using a custom method, expects a method with the signature object method(element)
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Reduce</mark>(<mark style="color:blue;">UserMethod</mark> <mark style="color:yellow;">method</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">initialValue</mark>)
Reduce the list using a custom method, expects a method with the signature object method(acc, element)
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Randomize</mark>()
Randomize the list
#### <mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">ToSet</mark>()
Convert the list to a set

---

