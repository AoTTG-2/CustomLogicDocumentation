# Random
Inherits from object
## Methods
#### <mark style="color:#509cd4;">int</mark> <mark style="color:#dcdcaa;">RandomInt</mark>(<mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">min</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">max</mark>)
Generates a random integer between the specified range.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">RandomFloat</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">min</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">max</mark>)
Generates a random float between the specified range.
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">RandomBool</mark>()
Returns random boolean.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">RandomVector3</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Generates a random Vector3 between the specified ranges.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">RandomDirection</mark>(<mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">flat</mark> = <mark style="color:#509cd4;">False</mark>)
Generates a random normalized direction vector. If flat is true, the y component will be zero.
#### <mark style="color:#509cd4;">int</mark> <mark style="color:#dcdcaa;">RandomSign</mark>()
Generates a random sign, either 1 or -1.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">PerlinNoise</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">x</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">y</mark>)
Returns a point sampled from generated 2d perlin noise. (see Unity Mathf.PerlinNoise for more information)

---

