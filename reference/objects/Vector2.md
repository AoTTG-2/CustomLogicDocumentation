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
#### void <span style="color":#dcdcaa>Set<span>(float <span style="color":#9cdcfe>x<span>, float <span style="color":#9cdcfe>y<span>)
Set x and y components of an existing Vector2.
#### void <span style="color":#dcdcaa>Normalize<span>()
Makes this vector have a magnitude of 1.
#### Object <span style="color":#dcdcaa>\_\_Copy\_\_<span>()
Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()
#### Object <span style="color":#dcdcaa>\_\_Add\_\_<span>(Object <span style="color":#9cdcfe>self<span>, Object <span style="color":#9cdcfe>other<span>)
Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)
#### Object <span style="color":#dcdcaa>\_\_Sub\_\_<span>(Object <span style="color":#9cdcfe>self<span>, Object <span style="color":#9cdcfe>other<span>)
Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)
#### Object <span style="color":#dcdcaa>\_\_Mul\_\_<span>(Object <span style="color":#9cdcfe>self<span>, Object <span style="color":#9cdcfe>other<span>)
Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)
#### Object <span style="color":#dcdcaa>\_\_Div\_\_<span>(Object <span style="color":#9cdcfe>self<span>, Object <span style="color":#9cdcfe>other<span>)
Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)
#### bool <span style="color":#dcdcaa>\_\_Eq\_\_<span>(Object <span style="color":#9cdcfe>self<span>, Object <span style="color":#9cdcfe>other<span>)
Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)
#### int <span style="color":#dcdcaa>\_\_Hash\_\_<span>()
Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()

---

## Static Methods
#### float <span style="color":#dcdcaa>Angle<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>from<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>to<span>)
Gets the unsigned angle in degrees between from and to.
#### [Vector2](../objects/Vector2.md) <span style="color":#dcdcaa>ClampMagnitude<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>vector<span>, float <span style="color":#9cdcfe>maxLength<span>)
Returns a copy of vector with its magnitude clamped to maxLength.
#### float <span style="color":#dcdcaa>Distance<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>a<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>b<span>)
Returns the distance between a and b.
#### float <span style="color":#dcdcaa>Dot<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>a<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>b<span>)
Dot Product of two vectors.
#### [Vector2](../objects/Vector2.md) <span style="color":#dcdcaa>Lerp<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>a<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>b<span>, float <span style="color":#9cdcfe>t<span>)
Linearly interpolates between vectors a and b by t.
#### [Vector2](../objects/Vector2.md) <span style="color":#dcdcaa>LerpUnclamped<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>a<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>b<span>, float <span style="color":#9cdcfe>t<span>)
Linearly interpolates between vectors a and b by t.
#### [Vector2](../objects/Vector2.md) <span style="color":#dcdcaa>Max<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>a<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>b<span>)
Returns a vector that is made from the largest components of two vectors.
#### [Vector2](../objects/Vector2.md) <span style="color":#dcdcaa>Min<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>a<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>b<span>)
Returns a vector that is made from the smallest components of two vectors.
#### [Vector2](../objects/Vector2.md) <span style="color":#dcdcaa>MoveTowards<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>current<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>target<span>, float <span style="color":#9cdcfe>maxDistanceDelta<span>)
Moves a point current towards target.
#### [Vector2](../objects/Vector2.md) <span style="color":#dcdcaa>Reflect<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>inDirection<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>inNormal<span>)
Reflects a vector off the vector defined by a normal.
#### float <span style="color":#dcdcaa>SignedAngle<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>from<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>to<span>)
Gets the signed angle in degrees between from and to.
#### [Vector2](../objects/Vector2.md) <span style="color":#dcdcaa>SmoothDamp<span>([Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>current<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>target<span>, [Vector2](../objects/Vector2.md) <span style="color":#9cdcfe>currentVelocity<span>, float <span style="color":#9cdcfe>smoothTime<span>, float <span style="color":#9cdcfe>maxSpeed<span>)


---

