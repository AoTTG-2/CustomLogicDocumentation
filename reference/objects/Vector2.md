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
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Set</mark>(<mark style="color:Blue;">float</mark> <mark style="color:Yellow;">x</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">y</mark>)
Set x and y components of an existing Vector2.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Normalize</mark>()
Makes this vector have a magnitude of 1.
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Copy\_\_</mark>()
Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Add\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Sub\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Mul\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Div\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">\_\_Eq\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)
#### <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">\_\_Hash\_\_</mark>()
Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()

---

## Static Methods
#### <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">Angle</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">from</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">to</mark>)
Gets the unsigned angle in degrees between from and to.
#### <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">ClampMagnitude</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">vector</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">maxLength</mark>)
Returns a copy of vector with its magnitude clamped to maxLength.
#### <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">Distance</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">b</mark>)
Returns the distance between a and b.
#### <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">Dot</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">b</mark>)
Dot Product of two vectors.
#### <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">Lerp</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">t</mark>)
Linearly interpolates between vectors a and b by t.
#### <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">LerpUnclamped</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">t</mark>)
Linearly interpolates between vectors a and b by t.
#### <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">Max</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">b</mark>)
Returns a vector that is made from the largest components of two vectors.
#### <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">Min</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">b</mark>)
Returns a vector that is made from the smallest components of two vectors.
#### <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">MoveTowards</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">current</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">target</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">maxDistanceDelta</mark>)
Moves a point current towards target.
#### <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">Reflect</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">inDirection</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">inNormal</mark>)
Reflects a vector off the vector defined by a normal.
#### <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">SignedAngle</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">from</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">to</mark>)
Gets the signed angle in degrees between from and to.
#### <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">SmoothDamp</mark>(<mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">current</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">target</mark>, <mark style="color:Blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:Yellow;">currentVelocity</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">smoothTime</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">maxSpeed</mark>)


---

