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

#### <mark style="color:blue;">void Clear()</mark>

Clear all set elements

#### bool Contains(Object value)

Check if the set contains the specified element

#### void Add(Object value)

Add an element to the set

#### void Remove(Object value)

Remove the element from the set

#### void Union([Set](Set.md) set)

Union with another set

#### void Intersect([Set](Set.md) set)

Intersect with another set

#### void Difference([Set](Set.md) set)

Difference with another set

#### bool IsSubsetOf([Set](Set.md) set)

Check if the set is a subset of another set

#### bool IsSupersetOf([Set](Set.md) set)

Check if the set is a superset of another set

#### bool IsProperSubsetOf([Set](Set.md) set)

Check if the set is a proper subset of another set

#### bool IsProperSupersetOf([Set](Set.md) set)

Check if the set is a proper superset of another set

#### bool Overlaps([Set](Set.md) set)

Check if the set overlaps with another set

#### bool SetEquals([Set](Set.md) set)

Check if the set has the same elements as another set

#### [List](List.md) ToList()

Convert the set to a list

***
