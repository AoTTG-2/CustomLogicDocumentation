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
|Function|Returns|Description|
|---|---|---|
|\_\_Copy\_\_()|Object|Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()|
|\_\_Add\_\_(<br/><i>self</i> : Object,<br/><i>other</i> : Object<br/>)|Object|Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)|
|\_\_Sub\_\_(<br/><i>self</i> : Object,<br/><i>other</i> : Object<br/>)|Object|Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)|
|\_\_Mul\_\_(<br/><i>self</i> : Object,<br/><i>other</i> : Object<br/>)|Object|Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)|
|\_\_Div\_\_(<br/><i>self</i> : Object,<br/><i>other</i> : Object<br/>)|Object|Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)|
|\_\_Eq\_\_(<br/><i>self</i> : Object,<br/><i>other</i> : Object<br/>)|bool|Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)|
|\_\_Hash\_\_()|int|Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()|
## Static Methods
|Function|Returns|Description|
|---|---|---|
|Lerp(<br/><i>a</i> : [Quaternion](../objects/Quaternion.md),<br/><i>b</i> : [Quaternion](../objects/Quaternion.md),<br/><i>t</i> : float<br/>)|[Quaternion](../objects/Quaternion.md)|Interpolates between a and b by t and normalizes the result afterwards.|
|LerpUnclamped(<br/><i>a</i> : [Quaternion](../objects/Quaternion.md),<br/><i>b</i> : [Quaternion](../objects/Quaternion.md),<br/><i>t</i> : float<br/>)|[Quaternion](../objects/Quaternion.md)|Interpolates between a and b by t and normalizes the result afterwards. The parameter t is not clamped.|
|Slerp(<br/><i>a</i> : [Quaternion](../objects/Quaternion.md),<br/><i>b</i> : [Quaternion](../objects/Quaternion.md),<br/><i>t</i> : float<br/>)|[Quaternion](../objects/Quaternion.md)|Spherically linear interpolates between unit quaternions a and b by a ratio of t.|
|SlerpUnclamped(<br/><i>a</i> : [Quaternion](../objects/Quaternion.md),<br/><i>b</i> : [Quaternion](../objects/Quaternion.md),<br/><i>t</i> : float<br/>)|[Quaternion](../objects/Quaternion.md)|Spherically linear interpolates between unit quaternions a and b by t.|
|FromEuler(<i>euler</i> : [Vector3](../objects/Vector3.md))|[Quaternion](../objects/Quaternion.md)|Returns the Quaternion rotation from the given euler angles.|
|LookRotation(<br/><i>forward</i> : [Vector3](../objects/Vector3.md),<br/><i>upwards</i> : [Vector3](../objects/Vector3.md) = <br/>)|[Quaternion](../objects/Quaternion.md)|Creates a rotation with the specified forward and upwards directions.|
|FromToRotation(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|[Quaternion](../objects/Quaternion.md)|Creates a rotation from fromDirection to toDirection.|
|Inverse(<i>q</i> : [Quaternion](../objects/Quaternion.md))|[Quaternion](../objects/Quaternion.md)|Returns the Inverse of rotation.|
|RotateTowards(<br/><i>from</i> : [Quaternion](../objects/Quaternion.md),<br/><i>to</i> : [Quaternion](../objects/Quaternion.md),<br/><i>maxDegreesDelta</i> : float<br/>)|[Quaternion](../objects/Quaternion.md)|Rotates a rotation from towards to.|
