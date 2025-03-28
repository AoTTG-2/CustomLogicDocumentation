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
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Copy\_\_</mark>()
Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Add\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Sub\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Mul\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">\_\_Div\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">\_\_Eq\_\_</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">self</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">other</mark>)
Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)
#### <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">\_\_Hash\_\_</mark>()
Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()

---

## Static Methods
#### <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">Lerp</mark>(<mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">t</mark>)
Interpolates between a and b by t and normalizes the result afterwards.
#### <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">LerpUnclamped</mark>(<mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">t</mark>)
Interpolates between a and b by t and normalizes the result afterwards. The parameter t is not clamped.
#### <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">Slerp</mark>(<mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">t</mark>)
Spherically linear interpolates between unit quaternions a and b by a ratio of t.
#### <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">SlerpUnclamped</mark>(<mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">t</mark>)
Spherically linear interpolates between unit quaternions a and b by t.
#### <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">FromEuler</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">euler</mark>)
Returns the Quaternion rotation from the given euler angles.
#### <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">LookRotation</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">forward</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">upwards</mark> = <mark style="color:Blue;">null</mark>)
Creates a rotation with the specified forward and upwards directions.
#### <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">FromToRotation</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">b</mark>)
Creates a rotation from fromDirection to toDirection.
#### <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">Inverse</mark>(<mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">q</mark>)
Returns the Inverse of rotation.
#### <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">RotateTowards</mark>(<mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">from</mark>, <mark style="color:Blue;">[Quaternion](../objects/Quaternion.md)</mark> <mark style="color:Yellow;">to</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">maxDegreesDelta</mark>)
Rotates a rotation from towards to.

---

