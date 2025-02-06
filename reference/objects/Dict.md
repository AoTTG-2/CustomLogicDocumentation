# Dict
Inherits from object
## Initialization
```csharp
example = Dict()
```
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Count|int|False|Number of elements in the dictionary|
|Keys|[List](../objects/List.md)|False|Keys in the dictionary|
|Values|[List](../objects/List.md)|False|Values in the dictionary|
## Methods
|Function|Returns|Description|
|---|---|---|
|Clear()|none|Clears the dictionary|
|Get(<br/><i>key</i> : Object,<br/><i>defaultValue</i> : Object = <br/>)|Object|Gets a value from the dictionary|
|Set(<br/><i>key</i> : Object,<br/><i>value</i> : Object<br/>)|none|Sets a value in the dictionary|
|Remove(<i>key</i> : Object)|none|Removes a value from the dictionary|
|Contains(<i>key</i> : Object)|bool|Checks if the dictionary contains a key|
