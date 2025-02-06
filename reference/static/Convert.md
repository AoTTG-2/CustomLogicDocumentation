# Convert
Inherits from object
## Methods
|Function|Returns|Description|
|---|---|---|
|ToFloat(<i>value</i> : Object)|float|Converts a value to a float|
|ToInt(<i>value</i> : Object)|int|Converts a value to an int|
|ToBool(<i>value</i> : Object)|bool|Converts a value to a bool|
|ToString(<i>value</i> : Object)|[String](../static/String.md)|Converts a value to a string|
|IsFloat(<i>value</i> : Object)|bool|Checks if the value is a float|
|IsInt(<i>value</i> : Object)|bool|Checks if the value is an int|
|IsBool(<i>value</i> : Object)|bool|Checks if the value is a bool|
|IsString(<i>value</i> : Object)|bool|Checks if the value is a string|
|IsObject(<i>value</i> : Object)|bool|Checks if the value is an object|
|IsList(<i>value</i> : Object)|bool|Checks if the value is a list|
|IsDict(<i>value</i> : Object)|bool|Checks if the value is a dictionary|
|HasVariable(<br/><i>cInstance</i> : CustomLogicClassInstance,<br/><i>variableName</i> : [String](../static/String.md)<br/>)|bool|Checks if the class instance has a variable|
|DefineVariable(<br/><i>cInstance</i> : CustomLogicClassInstance,<br/><i>variableName</i> : [String](../static/String.md),<br/><i>value</i> : Object<br/>)|none|Defines a variable for the class instance|
|RemoveVariable(<br/><i>cInstance</i> : CustomLogicClassInstance,<br/><i>variableName</i> : [String](../static/String.md)<br/>)|none|Removes a variable from the class instance|
|GetType(<i>cInstance</i> : CustomLogicClassInstance)|[String](../static/String.md)|Gets the type of the class instance|
