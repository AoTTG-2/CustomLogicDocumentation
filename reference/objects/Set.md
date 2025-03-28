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
#### void <span style="color":#dcdcaa>Clear<span>()
Clear all set elements
#### bool <span style="color":#dcdcaa>Contains<span>(Object <span style="color":#9cdcfe>value<span>)
Check if the set contains the specified element
#### void <span style="color":#dcdcaa>Add<span>(Object <span style="color":#9cdcfe>value<span>)
Add an element to the set
#### void <span style="color":#dcdcaa>Remove<span>(Object <span style="color":#9cdcfe>value<span>)
Remove the element from the set
#### void <span style="color":#dcdcaa>Union<span>([Set](../objects/Set.md) <span style="color":#9cdcfe>set<span>)
Union with another set
#### void <span style="color":#dcdcaa>Intersect<span>([Set](../objects/Set.md) <span style="color":#9cdcfe>set<span>)
Intersect with another set
#### void <span style="color":#dcdcaa>Difference<span>([Set](../objects/Set.md) <span style="color":#9cdcfe>set<span>)
Difference with another set
#### bool <span style="color":#dcdcaa>IsSubsetOf<span>([Set](../objects/Set.md) <span style="color":#9cdcfe>set<span>)
Check if the set is a subset of another set
#### bool <span style="color":#dcdcaa>IsSupersetOf<span>([Set](../objects/Set.md) <span style="color":#9cdcfe>set<span>)
Check if the set is a superset of another set
#### bool <span style="color":#dcdcaa>IsProperSubsetOf<span>([Set](../objects/Set.md) <span style="color":#9cdcfe>set<span>)
Check if the set is a proper subset of another set
#### bool <span style="color":#dcdcaa>IsProperSupersetOf<span>([Set](../objects/Set.md) <span style="color":#9cdcfe>set<span>)
Check if the set is a proper superset of another set
#### bool <span style="color":#dcdcaa>Overlaps<span>([Set](../objects/Set.md) <span style="color":#9cdcfe>set<span>)
Check if the set overlaps with another set
#### bool <span style="color":#dcdcaa>SetEquals<span>([Set](../objects/Set.md) <span style="color":#9cdcfe>set<span>)
Check if the set has the same elements as another set
#### [List](../objects/List.md) <span style="color":#dcdcaa>ToList<span>()
Convert the set to a list

---

