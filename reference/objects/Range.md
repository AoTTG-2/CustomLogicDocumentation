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
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Clear</span>()
Clear all list elements
#### <span style="color:#509cd4">Object</span> <span style="color:#dcdcaa">Get</span>(<span style="color:#509cd4">int</span> <span style="color:#9cdcfe">index</span>)
Get the element at the specified index
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Set</span>(<span style="color:#509cd4">int</span> <span style="color:#9cdcfe">index</span>, <span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">value</span>)
Set the element at the specified index
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Add</span>(<span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">value</span>)
Add an element to the end of the list
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">InsertAt</span>(<span style="color:#509cd4">int</span> <span style="color:#9cdcfe">index</span>, <span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">value</span>)
Insert an element at the specified index
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">RemoveAt</span>(<span style="color:#509cd4">int</span> <span style="color:#9cdcfe">index</span>)
Remove the element at the specified index
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Remove</span>(<span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">value</span>)
Remove the first occurrence of the specified element
#### <span style="color:#509cd4">bool</span> <span style="color:#dcdcaa">Contains</span>(<span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">value</span>)
Check if the list contains the specified element
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Sort</span>()
Sort the list
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SortCustom</span>(<span style="color:#509cd4">UserMethod</span> <span style="color:#9cdcfe">method</span>)
Sort the list using a custom method, expects a method with the signature int method(a,b)
#### <span style="color:#509cd4">[List](../objects/List.md)</span> <span style="color:#dcdcaa">Filter</span>(<span style="color:#509cd4">UserMethod</span> <span style="color:#9cdcfe">method</span>)
Filter the list using a custom method, expects a method with the signature bool method(element)
#### <span style="color:#509cd4">[List](../objects/List.md)</span> <span style="color:#dcdcaa">Map</span>(<span style="color:#509cd4">UserMethod</span> <span style="color:#9cdcfe">method</span>)
Map the list using a custom method, expects a method with the signature object method(element)
#### <span style="color:#509cd4">Object</span> <span style="color:#dcdcaa">Reduce</span>(<span style="color:#509cd4">UserMethod</span> <span style="color:#9cdcfe">method</span>, <span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">initialValue</span>)
Reduce the list using a custom method, expects a method with the signature object method(acc, element)
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Randomize</span>()
Randomize the list
#### <span style="color:#509cd4">[Set](../objects/Set.md)</span> <span style="color:#dcdcaa">ToSet</span>()
Convert the list to a set

---

