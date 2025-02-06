# Random
Inherits from object
## Methods
|Function|Returns|Description|
|---|---|---|
|RandomInt(<br/><i>min</i> : int,<br/><i>max</i> : int<br/>)|int|Generates a random integer between the specified range.|
|RandomFloat(<br/><i>min</i> : float,<br/><i>max</i> : float<br/>)|float|Generates a random float between the specified range.|
|RandomBool()|bool|Returns random boolean.|
|RandomVector3(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Generates a random Vector3 between the specified ranges.|
|RandomDirection(<i>flat</i> : bool = False)|[Vector3](../objects/Vector3.md)|Generates a random normalized direction vector. If flat is true, the y component will be zero.|
|RandomSign()|int|Generates a random sign, either 1 or -1.|
|PerlinNoise(<br/><i>x</i> : float,<br/><i>y</i> : float<br/>)|float|Returns a point sampled from generated 2d perlin noise. (see Unity Mathf.PerlinNoise for more information)|
