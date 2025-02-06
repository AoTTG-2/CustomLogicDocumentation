# Random
Inherits from object
## Methods
|Function|Returns|Description|
|---|---|---|
|RandomInt(<br/>min : int,<br/>max : int<br/>)|int|Generates a random integer between the specified range.|
|RandomFloat(<br/>min : float,<br/>max : float<br/>)|float|Generates a random float between the specified range.|
|RandomBool()|bool|Returns random boolean.|
|RandomVector3(<br/>a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Generates a random Vector3 between the specified ranges.|
|RandomDirection(flat : bool = False)|[Vector3](../objects/Vector3.md)|Generates a random normalized direction vector. If flat is true, the y component will be zero.|
|RandomSign()|int|Generates a random sign, either 1 or -1.|
|PerlinNoise(<br/>x : float,<br/>y : float<br/>)|float|Returns a point sampled from generated 2d perlin noise. (see Unity Mathf.PerlinNoise for more information)|
