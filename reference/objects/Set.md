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
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Clear</mark>()
Clear all set elements
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">Contains</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Check if the set contains the specified element
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Add</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Add an element to the set
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Remove</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Remove the element from the set
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Union</mark>(<mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">set</mark>)
Union with another set
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Intersect</mark>(<mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">set</mark>)
Intersect with another set
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Difference</mark>(<mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">set</mark>)
Difference with another set
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">IsSubsetOf</mark>(<mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">set</mark>)
Check if the set is a subset of another set
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">IsSupersetOf</mark>(<mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">set</mark>)
Check if the set is a superset of another set
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">IsProperSubsetOf</mark>(<mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">set</mark>)
Check if the set is a proper subset of another set
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">IsProperSupersetOf</mark>(<mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">set</mark>)
Check if the set is a proper superset of another set
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">Overlaps</mark>(<mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">set</mark>)
Check if the set overlaps with another set
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">SetEquals</mark>(<mark style="color:Blue;">[Set](../objects/Set.md)</mark> <mark style="color:Yellow;">set</mark>)
Check if the set has the same elements as another set
#### <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">ToList</mark>()

Convert the set to a list

---

