# Vector3
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|X|float|False|X component of the vector.|
|Y|float|False|Y component of the vector.|
|Z|float|False|Z component of the vector.|
|Normalized|[Vector3](../objects/Vector3.md)|False|Returns this vector with a magnitude of 1 (Read Only).|
|Magnitude|float|False|Returns the length of this vector (Read Only).|
|SqrMagnitude|float|False|Returns the squared length of this vector (Read Only).|
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Zero|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(0, 0, 0).|
|One|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(1, 1, 1).|
|Up|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(0, 1, 0).|
|Down|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(0, -1, 0).|
|Left|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(-1, 0, 0).|
|Right|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(1, 0, 0).|
|Forward|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(0, 0, 1).|
|Back|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(0, 0, -1).|
|NegativeInfinity|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(float.PositiveInfinity, float.PositiveInfinity, float.PositiveInfinity).|
|PositiveInfinity|[Vector3](../objects/Vector3.md)|False|Shorthand for writing Vector3(float.PositiveInfinity, float.PositiveInfinity, float.PositiveInfinity).|
## Methods
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Set</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">x</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">y</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">z</mark>)
Set x, y and z components of an existing Vector3.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Scale</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">scale</mark>)
Returns the Vector3 multiplied by scale.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Multiply</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Returns the multiplication of two Vector3s.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Divide</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Returns the division of two Vector3s.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">GetRotationDirection</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Gets the relational Vector3 "b" using "a" as a reference. This is equivalent to setting MapObject.Forward to Vector "a", and finding the relative "b" vector.
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
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">Angle</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">from</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">to</mark>)
Calculates the angle between vectors from and.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">ClampMagnitude</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">vector</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">maxLength</mark>)
Returns a copy of vector with its magnitude clamped to maxLength.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Cross</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Cross Product of two vectors.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">Distance</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Returns the distance between a and b.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">Dot</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Dot Product of two vectors.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Lerp</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">t</mark>)
Linearly interpolates between two points.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">LerpUnclamped</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">t</mark>)
Linearly interpolates between two vectors.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Max</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Returns a vector that is made from the largest components of two vectors.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Min</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Returns a vector that is made from the smallest components of two vectors.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">MoveTowards</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">current</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">maxDistanceDelta</mark>)
Calculate a position between the points specified by current and target, moving no farther than the distance specified by maxDistanceDelta.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Normalize</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">value</mark>)
Makes this vector have a magnitude of 1.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">OrthoNormalize</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)

#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Project</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>)
Projects a vector onto another vector.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">ProjectOnPlane</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">vector</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">plane</mark>)
Projects a vector onto a plane defined by a normal orthogonal to the plane.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Reflect</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">inDirection</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">inNormal</mark>)
Reflects a vector off the plane defined by a normal.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">RotateTowards</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">current</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">maxRadiansDelta</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">maxMagnitudeDelta</mark>)
Rotates a vector current towards target.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">SignedAngle</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">from</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">to</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">axis</mark>)
Calculates the signed angle between vectors from and to in relation to axis.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">Slerp</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">t</mark>)
Spherically interpolates between two vectors.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">SlerpUnclamped</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">t</mark>)
Spherically interpolates between two vectors.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">SmoothDamp</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">current</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">currentVelocity</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">smoothTime</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">maxSpeed</mark>)


---

