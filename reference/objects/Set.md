# Set

Inherits from object

## Initialization

```csharp
example = Set()
example = Set((CustomLogicListBuiltin))
```

## Fields

| Field | Type | Readonly | Description                       |
| ----- | ---- | -------- | --------------------------------- |
| Count | int  | True     | The number of elements in the set |

## Methods
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Clear</mark>()
Clear all set elements
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">Contains</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Check if the set contains the specified element
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Add</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Add an element to the set
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Remove</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Remove the element from the set
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Union</mark>(<mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">set</mark>)
Union with another set
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Intersect</mark>(<mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">set</mark>)
Intersect with another set
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Difference</mark>(<mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">set</mark>)
Difference with another set
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">IsSubsetOf</mark>(<mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">set</mark>)
Check if the set is a subset of another set
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">IsSupersetOf</mark>(<mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">set</mark>)
Check if the set is a superset of another set
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">IsProperSubsetOf</mark>(<mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">set</mark>)
Check if the set is a proper subset of another set
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">IsProperSupersetOf</mark>(<mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">set</mark>)
Check if the set is a proper superset of another set
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">Overlaps</mark>(<mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">set</mark>)
Check if the set overlaps with another set
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">SetEquals</mark>(<mark style="color:blue;">[Set](../objects/Set.md)</mark> <mark style="color:yellow;">set</mark>)
Check if the set has the same elements as another set
#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">ToList</mark>()
Convert the set to a list

<mark style="color:blue;">Convert the set to a list</mark>

***
