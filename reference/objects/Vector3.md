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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Set</mark>(<mark style="color:blue;">float</mark> x, <mark style="color:blue;">float</mark> y, <mark style="color:blue;">float</mark> z)
> Set x, y and z components of an existing Vector3.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Scale</mark>(<mark style="color:blue;">Object</mark> scale)
> <mark style="color:red;">This method is obselete</mark>

> **Note:** <mark style="color:green;">Use multiply operator instead</mark>

> Returns the Vector3 multiplied by scale.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Multiply</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> <mark style="color:red;">This method is obselete</mark>

> **Note:** <mark style="color:green;">Use multiply operator instead</mark>

> Returns the multiplication of two Vector3s.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Divide</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> <mark style="color:red;">This method is obselete</mark>

> **Note:** <mark style="color:green;">Use divide operator instead</mark>

> Returns the division of two Vector3s.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">GetRotationDirection</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> Gets the relational Vector3 "b" using "a" as a reference. This is equivalent to setting MapObject.Forward to Vector "a", and finding the relative "b" vector.

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Copy\_\_</mark>()
> Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Add\_\_</mark>(<mark style="color:blue;">Object</mark> self, <mark style="color:blue;">Object</mark> other)
> Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Sub\_\_</mark>(<mark style="color:blue;">Object</mark> self, <mark style="color:blue;">Object</mark> other)
> Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Mul\_\_</mark>(<mark style="color:blue;">Object</mark> self, <mark style="color:blue;">Object</mark> other)
> Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">\_\_Div\_\_</mark>(<mark style="color:blue;">Object</mark> self, <mark style="color:blue;">Object</mark> other)
> Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)

#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">\_\_Eq\_\_</mark>(<mark style="color:blue;">Object</mark> self, <mark style="color:blue;">Object</mark> other)
> Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)

#### <mark style="color:blue;">int</mark> <mark style="color:yellow;">\_\_Hash\_\_</mark>()
> Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()


---

## Static Methods
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Angle</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> from, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> to)
> Calculates the angle between vectors from and.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">ClampMagnitude</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> vector, <mark style="color:blue;">float</mark> maxLength)
> Returns a copy of vector with its magnitude clamped to maxLength.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Cross</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> Cross Product of two vectors.

#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Distance</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> Returns the distance between a and b.

#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Dot</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> Dot Product of two vectors.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Lerp</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b, <mark style="color:blue;">float</mark> t)
> Linearly interpolates between two points.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">LerpUnclamped</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b, <mark style="color:blue;">float</mark> t)
> Linearly interpolates between two vectors.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Max</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> Returns a vector that is made from the largest components of two vectors.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Min</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> Returns a vector that is made from the smallest components of two vectors.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">MoveTowards</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> current, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> target, <mark style="color:blue;">float</mark> maxDistanceDelta)
> Calculate a position between the points specified by current and target, moving no farther than the distance specified by maxDistanceDelta.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Normalize</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> value)
> Makes this vector have a magnitude of 1.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">OrthoNormalize</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> <mark style="color:red;">Missing description, please ping dev to fix this or if you need clarification :)</mark>

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Project</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b)
> Projects a vector onto another vector.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">ProjectOnPlane</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> vector, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> plane)
> Projects a vector onto a plane defined by a normal orthogonal to the plane.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Reflect</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> inDirection, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> inNormal)
> Reflects a vector off the plane defined by a normal.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">RotateTowards</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> current, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> target, <mark style="color:blue;">float</mark> maxRadiansDelta, <mark style="color:blue;">float</mark> maxMagnitudeDelta)
> Rotates a vector current towards target.

#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">SignedAngle</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> from, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> to, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> axis)
> Calculates the signed angle between vectors from and to in relation to axis.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">Slerp</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b, <mark style="color:blue;">float</mark> t)
> Spherically interpolates between two vectors.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">SlerpUnclamped</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> a, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> b, <mark style="color:blue;">float</mark> t)
> Spherically interpolates between two vectors.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">SmoothDamp</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> current, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> target, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> currentVelocity, <mark style="color:blue;">float</mark> smoothTime, <mark style="color:blue;">float</mark> maxSpeed)
> <mark style="color:red;">Missing description, please ping dev to fix this or if you need clarification :)</mark>


---

