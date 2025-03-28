# Random
Inherits from object
## Methods
#### <mark style="color:blue;">int</mark> <mark style="color:yellow;">RandomInt</mark>(<mark style="color:blue;">int</mark> <mark style="color:yellow;">min</mark>, <mark style="color:blue;">int</mark> <mark style="color:yellow;">max</mark>)
Generates a random integer between the specified range.
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">RandomFloat</mark>(<mark style="color:blue;">float</mark> <mark style="color:yellow;">min</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">max</mark>)
Generates a random float between the specified range.
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">RandomBool</mark>()
Returns random boolean.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">RandomVector3</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Generates a random Vector3 between the specified ranges.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">RandomDirection</mark>(<mark style="color:blue;">bool</mark> <mark style="color:yellow;">flat</mark> = <mark style="color:blue;">False</mark>)
Generates a random normalized direction vector. If flat is true, the y component will be zero.
#### <mark style="color:blue;">int</mark> <mark style="color:yellow;">RandomSign</mark>()
Generates a random sign, either 1 or -1.
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">PerlinNoise</mark>(<mark style="color:blue;">float</mark> <mark style="color:yellow;">x</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">y</mark>)
Returns a point sampled from generated 2d perlin noise. (see Unity Mathf.PerlinNoise for more information)

---

