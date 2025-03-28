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
#### <span style="color:blue;">void</span> <span style="color:yellow;">Set</span>(<span style="color:blue;">float</span> x, <span style="color:blue;">float</span> y, <span style="color:blue;">float</span> z)
> Set x, y and z components of an existing Vector3.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Scale</span>(<span style="color:blue;">Object</span> scale)
> Returns the Vector3 multiplied by scale.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Multiply</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Returns the multiplication of two Vector3s.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Divide</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Returns the division of two Vector3s.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">GetRotationDirection</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Gets the relational Vector3 "b" using "a" as a reference. This is equivalent to setting MapObject.Forward to Vector "a", and finding the relative "b" vector.
#### <span style="color:blue;">Object</span> <span style="color:yellow;">\_\_Copy\_\_</span>()
> Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()
#### <span style="color:blue;">Object</span> <span style="color:yellow;">\_\_Add\_\_</span>(<span style="color:blue;">Object</span> self, <span style="color:blue;">Object</span> other)
> Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)
#### <span style="color:blue;">Object</span> <span style="color:yellow;">\_\_Sub\_\_</span>(<span style="color:blue;">Object</span> self, <span style="color:blue;">Object</span> other)
> Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)
#### <span style="color:blue;">Object</span> <span style="color:yellow;">\_\_Mul\_\_</span>(<span style="color:blue;">Object</span> self, <span style="color:blue;">Object</span> other)
> Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)
#### <span style="color:blue;">Object</span> <span style="color:yellow;">\_\_Div\_\_</span>(<span style="color:blue;">Object</span> self, <span style="color:blue;">Object</span> other)
> Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)
#### <span style="color:blue;">bool</span> <span style="color:yellow;">\_\_Eq\_\_</span>(<span style="color:blue;">Object</span> self, <span style="color:blue;">Object</span> other)
> Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)
#### <span style="color:blue;">int</span> <span style="color:yellow;">\_\_Hash\_\_</span>()
> Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()

---

## Static Methods
#### <span style="color:blue;">float</span> <span style="color:yellow;">Angle</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> from, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> to)
> Calculates the angle between vectors from and.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">ClampMagnitude</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> vector, <span style="color:blue;">float</span> maxLength)
> Returns a copy of vector with its magnitude clamped to maxLength.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Cross</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Cross Product of two vectors.
#### <span style="color:blue;">float</span> <span style="color:yellow;">Distance</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Returns the distance between a and b.
#### <span style="color:blue;">float</span> <span style="color:yellow;">Dot</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Dot Product of two vectors.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Lerp</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b, <span style="color:blue;">float</span> t)
> Linearly interpolates between two points.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">LerpUnclamped</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b, <span style="color:blue;">float</span> t)
> Linearly interpolates between two vectors.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Max</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Returns a vector that is made from the largest components of two vectors.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Min</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Returns a vector that is made from the smallest components of two vectors.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">MoveTowards</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> current, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> target, <span style="color:blue;">float</span> maxDistanceDelta)
> Calculate a position between the points specified by current and target, moving no farther than the distance specified by maxDistanceDelta.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Normalize</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> value)
> Makes this vector have a magnitude of 1.
#### <span style="color:blue;">void</span> <span style="color:yellow;">OrthoNormalize</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> 
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Project</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Projects a vector onto another vector.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">ProjectOnPlane</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> vector, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> plane)
> Projects a vector onto a plane defined by a normal orthogonal to the plane.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Reflect</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> inDirection, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> inNormal)
> Reflects a vector off the plane defined by a normal.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">RotateTowards</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> current, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> target, <span style="color:blue;">float</span> maxRadiansDelta, <span style="color:blue;">float</span> maxMagnitudeDelta)
> Rotates a vector current towards target.
#### <span style="color:blue;">float</span> <span style="color:yellow;">SignedAngle</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> from, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> to, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> axis)
> Calculates the signed angle between vectors from and to in relation to axis.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">Slerp</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b, <span style="color:blue;">float</span> t)
> Spherically interpolates between two vectors.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">SlerpUnclamped</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b, <span style="color:blue;">float</span> t)
> Spherically interpolates between two vectors.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">SmoothDamp</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> current, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> target, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> currentVelocity, <span style="color:blue;">float</span> smoothTime, <span style="color:blue;">float</span> maxSpeed)
> 

---

