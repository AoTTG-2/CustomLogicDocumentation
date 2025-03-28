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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Set</mark>(<mark style="color:blue;">float</mark> <mark style="color:yellow;">x</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">y</mark>)
Set x and y components of an existing Vector2.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Normalize</mark>()
Makes this vector have a magnitude of 1.
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Copy\_\_</mark>()
Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Add\_\_</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">self</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">other</mark>)
Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Sub\_\_</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">self</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">other</mark>)
Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Mul\_\_</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">self</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">other</mark>)
Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Div\_\_</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">self</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">other</mark>)
Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">\_\_Eq\_\_</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">self</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">other</mark>)
Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)
#### <mark style="color:blue;">int</mark> <mark style="color:yellow;">\_\_Hash\_\_</mark>()
Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()

---

## Static Methods
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Angle</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">from</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">to</mark>)
Gets the unsigned angle in degrees between from and to.
#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">ClampMagnitude</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">vector</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">maxLength</mark>)
Returns a copy of vector with its magnitude clamped to maxLength.
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Distance</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">b</mark>)
Returns the distance between a and b.
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Dot</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">b</mark>)
Dot Product of two vectors.
#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">Lerp</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">t</mark>)
Linearly interpolates between vectors a and b by t.
#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">LerpUnclamped</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">t</mark>)
Linearly interpolates between vectors a and b by t.
#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">Max</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">b</mark>)
Returns a vector that is made from the largest components of two vectors.
#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">Min</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">b</mark>)
Returns a vector that is made from the smallest components of two vectors.
#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">MoveTowards</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">current</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">maxDistanceDelta</mark>)
Moves a point current towards target.
#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">Reflect</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">inDirection</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">inNormal</mark>)
Reflects a vector off the vector defined by a normal.
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">SignedAngle</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">from</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">to</mark>)
Gets the signed angle in degrees between from and to.
#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">SmoothDamp</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">current</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">currentVelocity</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">smoothTime</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">maxSpeed</mark>)


---

