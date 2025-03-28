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
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Clear</mark>()
Clear all list elements
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Get</mark>(<mark style="color:Blue;">int</mark> <mark style="color:Yellow;">index</mark>)
Get the element at the specified index
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Set</mark>(<mark style="color:Blue;">int</mark> <mark style="color:Yellow;">index</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Set the element at the specified index
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Add</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Add an element to the end of the list
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">InsertAt</mark>(<mark style="color:Blue;">int</mark> <mark style="color:Yellow;">index</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Insert an element at the specified index
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">RemoveAt</mark>(<mark style="color:Blue;">int</mark> <mark style="color:Yellow;">index</mark>)
Remove the element at the specified index
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Remove</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Remove the first occurrence of the specified element
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">Contains</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Check if the list contains the specified element
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Sort</mark>()
Sort the list
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SortCustom</mark>(<mark style="color:Blue;">UserMethod</mark> <mark style="color:Yellow;">method</mark>)
Sort the list using a custom method, expects a method with the signature int method(a,b)
#### <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">Filter</mark>(<mark style="color:Blue;">UserMethod</mark> <mark style="color:Yellow;">method</mark>)
Filter the list using a custom method, expects a method with the signature bool method(element)
#### <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">Map</mark>(<mark style="color:Blue;">UserMethod</mark> <mark style="color:Yellow;">method</mark>)
Map the list using a custom method, expects a method with the signature object method(element)
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Reduce</mark>(<mark style="color:Blue;">UserMethod</mark> <mark style="color:Yellow;">method</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">initialValue</mark>)
Reduce the list using a custom method, expects a method with the signature object method(acc, element)
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Randomize</mark>()
Randomize the list
#### <mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">ToSet</mark>()
Convert the list to a set

---

