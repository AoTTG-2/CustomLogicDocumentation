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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Set</mark>(<mark style="color:blue;">float</mark> <mark style="color:yellow;">x</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">y</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">z</mark>)
Set x, y and z components of an existing Vector3.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Scale</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">scale</mark>)
Returns the Vector3 multiplied by scale.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Multiply</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Returns the multiplication of two Vector3s.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Divide</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Returns the division of two Vector3s.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">GetRotationDirection</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Gets the relational Vector3 "b" using "a" as a reference. This is equivalent to setting MapObject.Forward to Vector "a", and finding the relative "b" vector.
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
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Angle</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">from</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">to</mark>)
Calculates the angle between vectors from and.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">ClampMagnitude</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">vector</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">maxLength</mark>)
Returns a copy of vector with its magnitude clamped to maxLength.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Cross</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Cross Product of two vectors.
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Distance</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Returns the distance between a and b.
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Dot</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Dot Product of two vectors.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Lerp</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">t</mark>)
Linearly interpolates between two points.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">LerpUnclamped</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">t</mark>)
Linearly interpolates between two vectors.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Max</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Returns a vector that is made from the largest components of two vectors.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Min</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Returns a vector that is made from the smallest components of two vectors.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">MoveTowards</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">current</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">maxDistanceDelta</mark>)
Calculate a position between the points specified by current and target, moving no farther than the distance specified by maxDistanceDelta.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Normalize</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">value</mark>)
Makes this vector have a magnitude of 1.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">OrthoNormalize</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Project</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>)
Projects a vector onto another vector.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">ProjectOnPlane</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">vector</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">plane</mark>)
Projects a vector onto a plane defined by a normal orthogonal to the plane.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Reflect</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">inDirection</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">inNormal</mark>)
Reflects a vector off the plane defined by a normal.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">RotateTowards</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">current</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">maxRadiansDelta</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">maxMagnitudeDelta</mark>)
Rotates a vector current towards target.
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">SignedAngle</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">from</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">to</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">axis</mark>)
Calculates the signed angle between vectors from and to in relation to axis.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Slerp</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">t</mark>)
Spherically interpolates between two vectors.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">SlerpUnclamped</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">t</mark>)
Spherically interpolates between two vectors.
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">SmoothDamp</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">current</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">currentVelocity</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">smoothTime</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">maxSpeed</mark>)


---

