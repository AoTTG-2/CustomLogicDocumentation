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
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Clear</mark>()
Clear all set elements
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">Contains</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Check if the set contains the specified element
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Add</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Add an element to the set
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Remove</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Remove the element from the set
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Union</mark>(<mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#9cdcfe;">set</mark>)
Union with another set
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Intersect</mark>(<mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#9cdcfe;">set</mark>)
Intersect with another set
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Difference</mark>(<mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#9cdcfe;">set</mark>)
Difference with another set
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">IsSubsetOf</mark>(<mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#9cdcfe;">set</mark>)
Check if the set is a subset of another set
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">IsSupersetOf</mark>(<mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#9cdcfe;">set</mark>)
Check if the set is a superset of another set
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">IsProperSubsetOf</mark>(<mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#9cdcfe;">set</mark>)
Check if the set is a proper subset of another set
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">IsProperSupersetOf</mark>(<mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#9cdcfe;">set</mark>)
Check if the set is a proper superset of another set
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">Overlaps</mark>(<mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#9cdcfe;">set</mark>)
Check if the set overlaps with another set
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">SetEquals</mark>(<mark style="color:#509cd4;">[Set](../objects/Set.md)</mark> <mark style="color:#9cdcfe;">set</mark>)
Check if the set has the same elements as another set
#### <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#dcdcaa;">ToList</mark>()
Convert the set to a list

---

