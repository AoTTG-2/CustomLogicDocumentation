# Set
Inherits from object
## Initialization
```csharp
example = Set()
example = Set((CustomLogicListBuiltin))
```
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Count|int|True|The number of elements in the set|
## Methods
#### <span style="color:blue;">void</span> <span style="color:yellow;">Clear</span>()
> Clear all set elements
#### <span style="color:blue;">bool</span> <span style="color:yellow;">Contains</span>(<span style="color:blue;">Object</span> value)
> Check if the set contains the specified element
#### <span style="color:blue;">void</span> <span style="color:yellow;">Add</span>(<span style="color:blue;">Object</span> value)
> Add an element to the set
#### <span style="color:blue;">void</span> <span style="color:yellow;">Remove</span>(<span style="color:blue;">Object</span> value)
> Remove the element from the set
#### <span style="color:blue;">void</span> <span style="color:yellow;">Union</span>(<span style="color:blue;">[Set](../objects/Set.md)</span> set)
> Union with another set
#### <span style="color:blue;">void</span> <span style="color:yellow;">Intersect</span>(<span style="color:blue;">[Set](../objects/Set.md)</span> set)
> Intersect with another set
#### <span style="color:blue;">void</span> <span style="color:yellow;">Difference</span>(<span style="color:blue;">[Set](../objects/Set.md)</span> set)
> Difference with another set
#### <span style="color:blue;">bool</span> <span style="color:yellow;">IsSubsetOf</span>(<span style="color:blue;">[Set](../objects/Set.md)</span> set)
> Check if the set is a subset of another set
#### <span style="color:blue;">bool</span> <span style="color:yellow;">IsSupersetOf</span>(<span style="color:blue;">[Set](../objects/Set.md)</span> set)
> Check if the set is a superset of another set
#### <span style="color:blue;">bool</span> <span style="color:yellow;">IsProperSubsetOf</span>(<span style="color:blue;">[Set](../objects/Set.md)</span> set)
> Check if the set is a proper subset of another set
#### <span style="color:blue;">bool</span> <span style="color:yellow;">IsProperSupersetOf</span>(<span style="color:blue;">[Set](../objects/Set.md)</span> set)
> Check if the set is a proper superset of another set
#### <span style="color:blue;">bool</span> <span style="color:yellow;">Overlaps</span>(<span style="color:blue;">[Set](../objects/Set.md)</span> set)
> Check if the set overlaps with another set
#### <span style="color:blue;">bool</span> <span style="color:yellow;">SetEquals</span>(<span style="color:blue;">[Set](../objects/Set.md)</span> set)
> Check if the set has the same elements as another set
#### <span style="color:blue;">[List](../objects/List.md)</span> <span style="color:yellow;">ToList</span>()
> Convert the set to a list

---

