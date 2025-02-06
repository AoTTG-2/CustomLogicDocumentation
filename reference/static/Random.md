# Random
Inherits from object
## Methods
|Function|Parameters|Returns|Description|
|---|---|---|---|
|RandomInt|min : int<br/>max : int|int|Generates a random integer between the specified range.|
|RandomFloat|min : float<br/>max : float|float|Generates a random float between the specified range.|
|RandomBool||bool|Returns random boolean.|
|RandomVector3|a : [Vector3](../objects/Vector3.md)<br/>b : [Vector3](../objects/Vector3.md)|[Vector3](../objects/Vector3.md)|Generates a random Vector3 between the specified ranges.|
|RandomDirection|flat : bool = False|[Vector3](../objects/Vector3.md)|Generates a random normalized direction vector. If flat is true, the y component will be zero.|
|RandomSign||int|Generates a random sign, either 1 or -1.|
|PerlinNoise|x : float<br/>y : float|float|Returns a point sampled from generated 2d perlin noise. (see Unity Mathf.PerlinNoise for more information)|
