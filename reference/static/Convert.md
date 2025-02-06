# Convert
Inherits from object
## Methods
|Function|Returns|Description|
|---|---|---|
|ToFloat(value : Object)|float|Converts a value to a float|
|ToInt(value : Object)|int|Converts a value to an int|
|ToBool(value : Object)|bool|Converts a value to a bool|
|ToString(value : Object)|[String](../static/String.md)|Converts a value to a string|
|IsFloat(value : Object)|bool|Checks if the value is a float|
|IsInt(value : Object)|bool|Checks if the value is an int|
|IsBool(value : Object)|bool|Checks if the value is a bool|
|IsString(value : Object)|bool|Checks if the value is a string|
|IsObject(value : Object)|bool|Checks if the value is an object|
|IsList(value : Object)|bool|Checks if the value is a list|
|IsDict(value : Object)|bool|Checks if the value is a dictionary|
|HasVariable(<br/>cInstance : CustomLogicClassInstance,<br/>variableName : [String](../static/String.md)<br/>)|bool|Checks if the class instance has a variable|
|DefineVariable(<br/>cInstance : CustomLogicClassInstance,<br/>variableName : [String](../static/String.md),<br/>value : Object<br/>)|none|Defines a variable for the class instance|
|RemoveVariable(<br/>cInstance : CustomLogicClassInstance,<br/>variableName : [String](../static/String.md)<br/>)|none|Removes a variable from the class instance|
|GetType(cInstance : CustomLogicClassInstance)|[String](../static/String.md)|Gets the type of the class instance|
