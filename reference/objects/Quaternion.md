# Quaternion
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|X|float|False|X component of the Quaternion. Don't modify this directly unless you know quaternions inside out.|
|Y|float|False|Y component of the Quaternion. Don't modify this directly unless you know quaternions inside out.|
|Z|float|False|Z component of the Quaternion. Don't modify this directly unless you know quaternions inside out.|
|W|float|False|W component of the Quaternion. Do not directly modify quaternions.|
|Euler|[Vector3](../objects/Vector3.md)|False|Returns or sets the euler angle representation of the rotation.|
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Identity|[Quaternion](../objects/Quaternion.md)|False|The identity rotation (Read Only).|
## Methods
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
#### <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:yellow;">Lerp</span>(<span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> a, <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> b, <span style="color:blue;">float</span> t)
> Interpolates between a and b by t and normalizes the result afterwards.
#### <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:yellow;">LerpUnclamped</span>(<span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> a, <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> b, <span style="color:blue;">float</span> t)
> Interpolates between a and b by t and normalizes the result afterwards. The parameter t is not clamped.
#### <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:yellow;">Slerp</span>(<span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> a, <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> b, <span style="color:blue;">float</span> t)
> Spherically linear interpolates between unit quaternions a and b by a ratio of t.
#### <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:yellow;">SlerpUnclamped</span>(<span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> a, <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> b, <span style="color:blue;">float</span> t)
> Spherically linear interpolates between unit quaternions a and b by t.
#### <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:yellow;">FromEuler</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> euler)
> Returns the Quaternion rotation from the given euler angles.
#### <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:yellow;">LookRotation</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> forward, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> upwards = <span style="color:blue;">null</span>)
> Creates a rotation with the specified forward and upwards directions.
#### <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:yellow;">FromToRotation</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> a, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> b)
> Creates a rotation from fromDirection to toDirection.
#### <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:yellow;">Inverse</span>(<span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> q)
> Returns the Inverse of rotation.
#### <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:yellow;">RotateTowards</span>(<span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> from, <span style="color:blue;">[Quaternion](../objects/Quaternion.md)</span> to, <span style="color:blue;">float</span> maxDegreesDelta)
> Rotates a rotation from towards to.

---

