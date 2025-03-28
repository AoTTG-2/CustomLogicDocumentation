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
#### <span style="color:blue;">void</span> <span style="color:yellow;">Set</span>(<span style="color:blue;">float</span> x, <span style="color:blue;">float</span> y)
> Set x and y components of an existing Vector2.
#### <span style="color:blue;">void</span> <span style="color:yellow;">Normalize</span>()
> Makes this vector have a magnitude of 1.
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
#### <span style="color:blue;">float</span> <span style="color:yellow;">Angle</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> from, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> to)
> Gets the unsigned angle in degrees between from and to.
#### <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> <span style="color:yellow;">ClampMagnitude</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> vector, <span style="color:blue;">float</span> maxLength)
> Returns a copy of vector with its magnitude clamped to maxLength.
#### <span style="color:blue;">float</span> <span style="color:yellow;">Distance</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> a, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> b)
> Returns the distance between a and b.
#### <span style="color:blue;">float</span> <span style="color:yellow;">Dot</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> a, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> b)
> Dot Product of two vectors.
#### <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> <span style="color:yellow;">Lerp</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> a, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> b, <span style="color:blue;">float</span> t)
> Linearly interpolates between vectors a and b by t.
#### <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> <span style="color:yellow;">LerpUnclamped</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> a, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> b, <span style="color:blue;">float</span> t)
> Linearly interpolates between vectors a and b by t.
#### <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> <span style="color:yellow;">Max</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> a, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> b)
> Returns a vector that is made from the largest components of two vectors.
#### <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> <span style="color:yellow;">Min</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> a, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> b)
> Returns a vector that is made from the smallest components of two vectors.
#### <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> <span style="color:yellow;">MoveTowards</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> current, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> target, <span style="color:blue;">float</span> maxDistanceDelta)
> Moves a point current towards target.
#### <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> <span style="color:yellow;">Reflect</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> inDirection, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> inNormal)
> Reflects a vector off the vector defined by a normal.
#### <span style="color:blue;">float</span> <span style="color:yellow;">SignedAngle</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> from, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> to)
> Gets the signed angle in degrees between from and to.
#### <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> <span style="color:yellow;">SmoothDamp</span>(<span style="color:blue;">[Vector2](../objects/Vector2.md)</span> current, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> target, <span style="color:blue;">[Vector2](../objects/Vector2.md)</span> currentVelocity, <span style="color:blue;">float</span> smoothTime, <span style="color:blue;">float</span> maxSpeed)
> 

---

