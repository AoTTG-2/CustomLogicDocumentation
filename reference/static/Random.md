# Random
Inherits from object
## Methods
#### <span style="color:#509cd4">int</span> <span style="color:#dcdcaa">RandomInt</span>(<span style="color:#509cd4">int</span> <span style="color:#9cdcfe">min</span>, <span style="color:#509cd4">int</span> <span style="color:#9cdcfe">max</span>)
Generates a random integer between the specified range.
#### <span style="color:#509cd4">float</span> <span style="color:#dcdcaa">RandomFloat</span>(<span style="color:#509cd4">float</span> <span style="color:#9cdcfe">min</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">max</span>)
Generates a random float between the specified range.
#### <span style="color:#509cd4">bool</span> <span style="color:#dcdcaa">RandomBool</span>()
Returns random boolean.
#### <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa">RandomVector3</span>(<span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">a</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">b</span>)
Generates a random Vector3 between the specified ranges.
#### <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa">RandomDirection</span>(<span style="color:#509cd4">bool</span> <span style="color:#9cdcfe">flat</span> = <span style="color:#509cd4">False</span>)
Generates a random normalized direction vector. If flat is true, the y component will be zero.
#### <span style="color:#509cd4">int</span> <span style="color:#dcdcaa">RandomSign</span>()
Generates a random sign, either 1 or -1.
#### <span style="color:#509cd4">float</span> <span style="color:#dcdcaa">PerlinNoise</span>(<span style="color:#509cd4">float</span> <span style="color:#9cdcfe">x</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">y</span>)
Returns a point sampled from generated 2d perlin noise. (see Unity Mathf.PerlinNoise for more information)

---

