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
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Clear</span>()
Clear all set elements
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">Contains</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Check if the set contains the specified element
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Add</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Add an element to the set
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Remove</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Remove the element from the set
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Union</span>(<span style="color:#509cd4;">[Set](../objects/Set.md)</span> <span style="color:#9cdcfe;">set</span>)
Union with another set
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Intersect</span>(<span style="color:#509cd4;">[Set](../objects/Set.md)</span> <span style="color:#9cdcfe;">set</span>)
Intersect with another set
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Difference</span>(<span style="color:#509cd4;">[Set](../objects/Set.md)</span> <span style="color:#9cdcfe;">set</span>)
Difference with another set
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">IsSubsetOf</span>(<span style="color:#509cd4;">[Set](../objects/Set.md)</span> <span style="color:#9cdcfe;">set</span>)
Check if the set is a subset of another set
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">IsSupersetOf</span>(<span style="color:#509cd4;">[Set](../objects/Set.md)</span> <span style="color:#9cdcfe;">set</span>)
Check if the set is a superset of another set
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">IsProperSubsetOf</span>(<span style="color:#509cd4;">[Set](../objects/Set.md)</span> <span style="color:#9cdcfe;">set</span>)
Check if the set is a proper subset of another set
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">IsProperSupersetOf</span>(<span style="color:#509cd4;">[Set](../objects/Set.md)</span> <span style="color:#9cdcfe;">set</span>)
Check if the set is a proper superset of another set
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">Overlaps</span>(<span style="color:#509cd4;">[Set](../objects/Set.md)</span> <span style="color:#9cdcfe;">set</span>)
Check if the set overlaps with another set
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">SetEquals</span>(<span style="color:#509cd4;">[Set](../objects/Set.md)</span> <span style="color:#9cdcfe;">set</span>)
Check if the set has the same elements as another set
#### <span style="color:#509cd4;">[List](../objects/List.md)</span> <span style="color:#dcdcaa;">ToList</span>()
Convert the set to a list

---

