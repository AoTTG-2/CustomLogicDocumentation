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
#### [Quaternion](../objects/Quaternion.md) <span style="color":#dcdcaa>Lerp<span>([Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>a<span>, [Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>b<span>, float <span style="color":#9cdcfe>t<span>)
Interpolates between a and b by t and normalizes the result afterwards.
#### [Quaternion](../objects/Quaternion.md) <span style="color":#dcdcaa>LerpUnclamped<span>([Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>a<span>, [Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>b<span>, float <span style="color":#9cdcfe>t<span>)
Interpolates between a and b by t and normalizes the result afterwards. The parameter t is not clamped.
#### [Quaternion](../objects/Quaternion.md) <span style="color":#dcdcaa>Slerp<span>([Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>a<span>, [Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>b<span>, float <span style="color":#9cdcfe>t<span>)
Spherically linear interpolates between unit quaternions a and b by a ratio of t.
#### [Quaternion](../objects/Quaternion.md) <span style="color":#dcdcaa>SlerpUnclamped<span>([Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>a<span>, [Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>b<span>, float <span style="color":#9cdcfe>t<span>)
Spherically linear interpolates between unit quaternions a and b by t.
#### [Quaternion](../objects/Quaternion.md) <span style="color":#dcdcaa>FromEuler<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>euler<span>)
Returns the Quaternion rotation from the given euler angles.
#### [Quaternion](../objects/Quaternion.md) <span style="color":#dcdcaa>LookRotation<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>forward<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>upwards<span> = null)
Creates a rotation with the specified forward and upwards directions.
#### [Quaternion](../objects/Quaternion.md) <span style="color":#dcdcaa>FromToRotation<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>a<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>b<span>)
Creates a rotation from fromDirection to toDirection.
#### [Quaternion](../objects/Quaternion.md) <span style="color":#dcdcaa>Inverse<span>([Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>q<span>)
Returns the Inverse of rotation.
#### [Quaternion](../objects/Quaternion.md) <span style="color":#dcdcaa>RotateTowards<span>([Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>from<span>, [Quaternion](../objects/Quaternion.md) <span style="color":#9cdcfe>to<span>, float <span style="color":#9cdcfe>maxDegreesDelta<span>)
Rotates a rotation from towards to.

---

