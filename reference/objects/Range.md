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
#### <span style="color:blue;">void</span> <span style="color:yellow;">Clear</span>()
> Clear all list elements
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Get</span>(<span style="color:blue;">int</span> index)
> Get the element at the specified index
#### <span style="color:blue;">void</span> <span style="color:yellow;">Set</span>(<span style="color:blue;">int</span> index, <span style="color:blue;">Object</span> value)
> Set the element at the specified index
#### <span style="color:blue;">void</span> <span style="color:yellow;">Add</span>(<span style="color:blue;">Object</span> value)
> Add an element to the end of the list
#### <span style="color:blue;">void</span> <span style="color:yellow;">InsertAt</span>(<span style="color:blue;">int</span> index, <span style="color:blue;">Object</span> value)
> Insert an element at the specified index
#### <span style="color:blue;">void</span> <span style="color:yellow;">RemoveAt</span>(<span style="color:blue;">int</span> index)
> Remove the element at the specified index
#### <span style="color:blue;">void</span> <span style="color:yellow;">Remove</span>(<span style="color:blue;">Object</span> value)
> Remove the first occurrence of the specified element
#### <span style="color:blue;">bool</span> <span style="color:yellow;">Contains</span>(<span style="color:blue;">Object</span> value)
> Check if the list contains the specified element
#### <span style="color:blue;">void</span> <span style="color:yellow;">Sort</span>()
> Sort the list
#### <span style="color:blue;">void</span> <span style="color:yellow;">SortCustom</span>(<span style="color:blue;">UserMethod</span> method)
> Sort the list using a custom method, expects a method with the signature int method(a,b)
#### <span style="color:blue;">[List](../objects/List.md)</span> <span style="color:yellow;">Filter</span>(<span style="color:blue;">UserMethod</span> method)
> Filter the list using a custom method, expects a method with the signature bool method(element)
#### <span style="color:blue;">[List](../objects/List.md)</span> <span style="color:yellow;">Map</span>(<span style="color:blue;">UserMethod</span> method)
> Map the list using a custom method, expects a method with the signature object method(element)
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Reduce</span>(<span style="color:blue;">UserMethod</span> method, <span style="color:blue;">Object</span> initialValue)
> Reduce the list using a custom method, expects a method with the signature object method(acc, element)
#### <span style="color:blue;">void</span> <span style="color:yellow;">Randomize</span>()
> Randomize the list
#### <span style="color:blue;">[Set](../objects/Set.md)</span> <span style="color:yellow;">ToSet</span>()
> Convert the list to a set

---

