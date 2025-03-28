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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Set</mark>(<mark style="color:blue;">float</mark> x, <mark style="color:blue;">float</mark> y)
> Set x and y components of an existing Vector2.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Normalize</mark>()
> Makes this vector have a magnitude of 1.

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
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Angle</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> from, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> to)
> Gets the unsigned angle in degrees between from and to.

#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">ClampMagnitude</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> vector, <mark style="color:blue;">float</mark> maxLength)
> Returns a copy of vector with its magnitude clamped to maxLength.

#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Distance</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> a, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> b)
> Returns the distance between a and b.

#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">Dot</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> a, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> b)
> Dot Product of two vectors.

#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">Lerp</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> a, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> b, <mark style="color:blue;">float</mark> t)
> Linearly interpolates between vectors a and b by t.

#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">LerpUnclamped</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> a, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> b, <mark style="color:blue;">float</mark> t)
> Linearly interpolates between vectors a and b by t.

#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">Max</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> a, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> b)
> Returns a vector that is made from the largest components of two vectors.

#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">Min</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> a, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> b)
> Returns a vector that is made from the smallest components of two vectors.

#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">MoveTowards</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> current, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> target, <mark style="color:blue;">float</mark> maxDistanceDelta)
> Moves a point current towards target.

#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">Reflect</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> inDirection, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> inNormal)
> Reflects a vector off the vector defined by a normal.

#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">SignedAngle</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> from, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> to)
> Gets the signed angle in degrees between from and to.

#### <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> <mark style="color:yellow;">SmoothDamp</mark>(<mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> current, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> target, <mark style="color:blue;">[Vector2](../objects/Vector2.md)</mark> currentVelocity, <mark style="color:blue;">float</mark> smoothTime, <mark style="color:blue;">float</mark> maxSpeed)
> <mark style="color:red;">Missing description, please ping dev to fix this or if you need clarification :)</mark>


---

