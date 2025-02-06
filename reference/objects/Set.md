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
|Function|Returns|Description|
|---|---|---|
|Clear()|none|Clear all set elements|
|Contains(<i>value</i> : Object)|bool|Check if the set contains the specified element|
|Add(<i>value</i> : Object)|none|Add an element to the set|
|Remove(<i>value</i> : Object)|none|Remove the element from the set|
|Union(<i>set</i> : [Set](../objects/Set.md))|none|Union with another set|
|Intersect(<i>set</i> : [Set](../objects/Set.md))|none|Intersect with another set|
|Difference(<i>set</i> : [Set](../objects/Set.md))|none|Difference with another set|
|IsSubsetOf(<i>set</i> : [Set](../objects/Set.md))|bool|Check if the set is a subset of another set|
|IsSupersetOf(<i>set</i> : [Set](../objects/Set.md))|bool|Check if the set is a superset of another set|
|IsProperSubsetOf(<i>set</i> : [Set](../objects/Set.md))|bool|Check if the set is a proper subset of another set|
|IsProperSupersetOf(<i>set</i> : [Set](../objects/Set.md))|bool|Check if the set is a proper superset of another set|
|Overlaps(<i>set</i> : [Set](../objects/Set.md))|bool|Check if the set overlaps with another set|
|SetEquals(<i>set</i> : [Set](../objects/Set.md))|bool|Check if the set has the same elements as another set|
|ToList()|[List](../objects/List.md)|Convert the set to a list|
