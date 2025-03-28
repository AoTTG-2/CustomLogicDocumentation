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
#### <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#dcdcaa;">Lerp</span>(<span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">t</span>)
Interpolates between a and b by t and normalizes the result afterwards.
#### <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#dcdcaa;">LerpUnclamped</span>(<span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">t</span>)
Interpolates between a and b by t and normalizes the result afterwards. The parameter t is not clamped.
#### <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#dcdcaa;">Slerp</span>(<span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">t</span>)
Spherically linear interpolates between unit quaternions a and b by a ratio of t.
#### <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#dcdcaa;">SlerpUnclamped</span>(<span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">t</span>)
Spherically linear interpolates between unit quaternions a and b by t.
#### <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#dcdcaa;">FromEuler</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">euler</span>)
Returns the Quaternion rotation from the given euler angles.
#### <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#dcdcaa;">LookRotation</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">forward</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">upwards</span> = <span style="color:#509cd4;">null</span>)
Creates a rotation with the specified forward and upwards directions.
#### <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#dcdcaa;">FromToRotation</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">b</span>)
Creates a rotation from fromDirection to toDirection.
#### <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#dcdcaa;">Inverse</span>(<span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">q</span>)
Returns the Inverse of rotation.
#### <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#dcdcaa;">RotateTowards</span>(<span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">from</span>, <span style="color:#509cd4;">[Quaternion](../objects/Quaternion.md)</span> <span style="color:#9cdcfe;">to</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">maxDegreesDelta</span>)
Rotates a rotation from towards to.

---

