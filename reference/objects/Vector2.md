# Vector2
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|X|float|False|X component of the vector.|
|Y|float|False|Y component of the vector.|
|Normalized|[Vector2](../objects/Vector2.md)|False|Returns this vector with a magnitude of 1 (Read Only).|
|Magnitude|float|False|Returns the length of this vector (Read Only).|
|SqrMagnitude|float|False|Returns the squared length of this vector (Read Only).|
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Zero|[Vector2](../objects/Vector2.md)|False|Shorthand for writing Vector2(0, 0).|
|One|[Vector2](../objects/Vector2.md)|False|Shorthand for writing Vector2(1, 1).|
|Up|[Vector2](../objects/Vector2.md)|False|Shorthand for writing Vector2(0, 1).|
|Down|[Vector2](../objects/Vector2.md)|False|Shorthand for writing Vector2(0, -1).|
|Left|[Vector2](../objects/Vector2.md)|False|Shorthand for writing Vector2(-1, 0).|
|Right|[Vector2](../objects/Vector2.md)|False|Shorthand for writing Vector2(1, 0).|
|NegativeInfinity|[Vector2](../objects/Vector2.md)|False|Shorthand for writing Vector2(float.PositiveInfinity, float.PositiveInfinity).|
|PositiveInfinity|[Vector2](../objects/Vector2.md)|False|Shorthand for writing Vector2(float.PositiveInfinity, float.PositiveInfinity).|
## Methods
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Set</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">x</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">y</mark>)
Set x and y components of an existing Vector2.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Normalize</mark>()
Makes this vector have a magnitude of 1.
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">\_\_Copy\_\_</mark>()
Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">\_\_Add\_\_</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">self</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">other</mark>)
Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">\_\_Sub\_\_</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">self</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">other</mark>)
Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">\_\_Mul\_\_</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">self</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">other</mark>)
Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">\_\_Div\_\_</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">self</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">other</mark>)
Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">\_\_Eq\_\_</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">self</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">other</mark>)
Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)
#### <mark style="color:#509cd4;">int</mark> <mark style="color:#dcdcaa;">\_\_Hash\_\_</mark>()
Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()

---

## Static Methods
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">Angle</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">from</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">to</mark>)
Gets the unsigned angle in degrees between from and to.
#### <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#dcdcaa;">ClampMagnitude</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">vector</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">maxLength</mark>)
Returns a copy of vector with its magnitude clamped to maxLength.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">Distance</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Returns the distance between a and b.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">Dot</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Dot Product of two vectors.
#### <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#dcdcaa;">Lerp</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">t</mark>)
Linearly interpolates between vectors a and b by t.
#### <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#dcdcaa;">LerpUnclamped</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">t</mark>)
Linearly interpolates between vectors a and b by t.
#### <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#dcdcaa;">Max</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Returns a vector that is made from the largest components of two vectors.
#### <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#dcdcaa;">Min</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Returns a vector that is made from the smallest components of two vectors.
#### <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#dcdcaa;">MoveTowards</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">current</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">maxDistanceDelta</mark>)
Moves a point current towards target.
#### <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#dcdcaa;">Reflect</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">inDirection</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">inNormal</mark>)
Reflects a vector off the vector defined by a normal.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">SignedAngle</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">from</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">to</mark>)
Gets the signed angle in degrees between from and to.
#### <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#dcdcaa;">SmoothDamp</mark>(<mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">current</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:#9cdcfe;">currentVelocity</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">smoothTime</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">maxSpeed</mark>)


---

