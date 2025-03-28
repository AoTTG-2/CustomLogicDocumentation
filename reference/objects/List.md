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
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Clear</mark>()
Clear all list elements
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Get</mark>(<mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">index</mark>)
Get the element at the specified index
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Set</mark>(<mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">index</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Set the element at the specified index
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Add</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Add an element to the end of the list
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">InsertAt</mark>(<mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">index</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Insert an element at the specified index
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">RemoveAt</mark>(<mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">index</mark>)
Remove the element at the specified index
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Remove</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Remove the first occurrence of the specified element
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">Contains</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Check if the list contains the specified element
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Sort</mark>()
Sort the list
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SortCustom</mark>(<mark style="color:#509cd4;">UserMethod</mark> <mark style="color:#9cdcfe;">method</mark>)
Sort the list using a custom method, expects a method with the signature int method(a,b)
#### <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#dcdcaa;">Filter</mark>(<mark style="color:#509cd4;">UserMethod</mark> <mark style="color:#9cdcfe;">method</mark>)
Filter the list using a custom method, expects a method with the signature bool method(element)
#### <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#dcdcaa;">Map</mark>(<mark style="color:#509cd4;">UserMethod</mark> <mark style="color:#9cdcfe;">method</mark>)
Map the list using a custom method, expects a method with the signature object method(element)
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Reduce</mark>(<mark style="color:#509cd4;">UserMethod</mark> <mark style="color:#9cdcfe;">method</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">initialValue</mark>)
Reduce the list using a custom method, expects a method with the signature object method(acc, element)
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Randomize</mark>()
Randomize the list
#### <mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#dcdcaa;">ToSet</mark>()
Convert the list to a set

---

