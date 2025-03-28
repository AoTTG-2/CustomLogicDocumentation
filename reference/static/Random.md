# Random
Inherits from object
## Methods
#### <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">RandomInt</mark>(<mark style="color:Blue;">int</mark> <mark style="color:Yellow;">min</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">max</mark>)
Generates a random integer between the specified range.
#### <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">RandomFloat</mark>(<mark style="color:Blue;">float</mark> <mark style="color:Yellow;">min</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">max</mark>)
Generates a random float between the specified range.
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">RandomBool</mark>()
Returns random boolean.
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">RandomVector3</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">b</mark>)
Generates a random Vector3 between the specified ranges.
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">RandomDirection</mark>(<mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">flat</mark> = <mark style="color:Blue;">False</mark>)
Generates a random normalized direction vector. If flat is true, the y component will be zero.
#### <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">RandomSign</mark>()
Generates a random sign, either 1 or -1.
#### <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">PerlinNoise</mark>(<mark style="color:Blue;">float</mark> <mark style="color:Yellow;">x</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">y</mark>)
Returns a point sampled from generated 2d perlin noise. (see Unity Mathf.PerlinNoise for more information)

---

