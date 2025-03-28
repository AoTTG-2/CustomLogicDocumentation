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
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Set</span>(<span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">x</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">y</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">z</span>)
Set x, y and z components of an existing Vector3.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Scale</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">scale</span>)
Returns the Vector3 multiplied by scale.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Multiply</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Returns the multiplication of two Vector3s.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Divide</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Returns the division of two Vector3s.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">GetRotationDirection</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Gets the relational Vector3 "b" using "a" as a reference. This is equivalent to setting MapObject.Forward to Vector "a", and finding the relative "b" vector.
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">\_\_Copy\_\_</span>()
Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">\_\_Add\_\_</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">self</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">other</span>)
Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">\_\_Sub\_\_</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">self</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">other</span>)
Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">\_\_Mul\_\_</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">self</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">other</span>)
Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">\_\_Div\_\_</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">self</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">other</span>)
Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">\_\_Eq\_\_</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">self</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">other</span>)
Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)
#### <span style="color:#509cd4;">int</span> <span style="color:#dcdcaa;">\_\_Hash\_\_</span>()
Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()

---

## Static Methods
#### <span style="color:#509cd4;">float</span> <span style="color:#dcdcaa;">Angle</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">from</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">to</span>)
Calculates the angle between vectors from and.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">ClampMagnitude</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">vector</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">maxLength</span>)
Returns a copy of vector with its magnitude clamped to maxLength.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Cross</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Cross Product of two vectors.
#### <span style="color:#509cd4;">float</span> <span style="color:#dcdcaa;">Distance</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Returns the distance between a and b.
#### <span style="color:#509cd4;">float</span> <span style="color:#dcdcaa;">Dot</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Dot Product of two vectors.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Lerp</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">t</span>)
Linearly interpolates between two points.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">LerpUnclamped</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">t</span>)
Linearly interpolates between two vectors.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Max</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Returns a vector that is made from the largest components of two vectors.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Min</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Returns a vector that is made from the smallest components of two vectors.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">MoveTowards</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">current</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">target</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">maxDistanceDelta</span>)
Calculate a position between the points specified by current and target, moving no farther than the distance specified by maxDistanceDelta.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Normalize</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">value</span>)
Makes this vector have a magnitude of 1.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">OrthoNormalize</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)

#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Project</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Projects a vector onto another vector.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">ProjectOnPlane</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">vector</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">plane</span>)
Projects a vector onto a plane defined by a normal orthogonal to the plane.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Reflect</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">inDirection</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">inNormal</span>)
Reflects a vector off the plane defined by a normal.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">RotateTowards</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">current</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">target</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">maxRadiansDelta</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">maxMagnitudeDelta</span>)
Rotates a vector current towards target.
#### <span style="color:#509cd4;">float</span> <span style="color:#dcdcaa;">SignedAngle</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">from</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">to</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">axis</span>)
Calculates the signed angle between vectors from and to in relation to axis.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">Slerp</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">t</span>)
Spherically interpolates between two vectors.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">SlerpUnclamped</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">t</span>)
Spherically interpolates between two vectors.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">SmoothDamp</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">current</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">target</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">currentVelocity</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">smoothTime</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">maxSpeed</span>)


---

