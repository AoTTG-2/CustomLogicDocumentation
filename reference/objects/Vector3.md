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
|Function|Returns|Description|
|---|---|---|
|Set(<br/><i>x</i> : float,<br/><i>y</i> : float,<br/><i>z</i> : float<br/>)|none|Set x, y and z components of an existing Vector3.|
|Scale(<i>scale</i> : Object)|[Vector3](../objects/Vector3.md)|Returns the Vector3 multiplied by scale.|
|Multiply(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Returns the multiplication of two Vector3s.|
|Divide(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Returns the division of two Vector3s.|
|GetRotationDirection(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Gets the relational Vector3 "b" using "a" as a reference. This is equivalent to setting MapObject.Forward to Vector "a", and finding the relative "b" vector.|
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
|Angle(<br/><i>from</i> : [Vector3](../objects/Vector3.md),<br/><i>to</i> : [Vector3](../objects/Vector3.md)<br/>)|float|Calculates the angle between vectors from and.|
|ClampMagnitude(<br/><i>vector</i> : [Vector3](../objects/Vector3.md),<br/><i>maxLength</i> : float<br/>)|[Vector3](../objects/Vector3.md)|Returns a copy of vector with its magnitude clamped to maxLength.|
|Cross(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Cross Product of two vectors.|
|Distance(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|float|Returns the distance between a and b.|
|Dot(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|float|Dot Product of two vectors.|
|Lerp(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md),<br/><i>t</i> : float<br/>)|[Vector3](../objects/Vector3.md)|Linearly interpolates between two points.|
|LerpUnclamped(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md),<br/><i>t</i> : float<br/>)|[Vector3](../objects/Vector3.md)|Linearly interpolates between two vectors.|
|Max(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Returns a vector that is made from the largest components of two vectors.|
|Min(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Returns a vector that is made from the smallest components of two vectors.|
|MoveTowards(<br/><i>current</i> : [Vector3](../objects/Vector3.md),<br/><i>target</i> : [Vector3](../objects/Vector3.md),<br/><i>maxDistanceDelta</i> : float<br/>)|[Vector3](../objects/Vector3.md)|Calculate a position between the points specified by current and target, moving no farther than the distance specified by maxDistanceDelta.|
|Normalize(<i>value</i> : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Makes this vector have a magnitude of 1.|
|OrthoNormalize(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|none||
|Project(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Projects a vector onto another vector.|
|ProjectOnPlane(<br/><i>vector</i> : [Vector3](../objects/Vector3.md),<br/><i>plane</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Projects a vector onto a plane defined by a normal orthogonal to the plane.|
|Reflect(<br/><i>inDirection</i> : [Vector3](../objects/Vector3.md),<br/><i>inNormal</i> : [Vector3](../objects/Vector3.md)<br/>)|[Vector3](../objects/Vector3.md)|Reflects a vector off the plane defined by a normal.|
|RotateTowards(<br/><i>current</i> : [Vector3](../objects/Vector3.md),<br/><i>target</i> : [Vector3](../objects/Vector3.md),<br/><i>maxRadiansDelta</i> : float,<br/><i>maxMagnitudeDelta</i> : float<br/>)|[Vector3](../objects/Vector3.md)|Rotates a vector current towards target.|
|SignedAngle(<br/><i>from</i> : [Vector3](../objects/Vector3.md),<br/><i>to</i> : [Vector3](../objects/Vector3.md),<br/><i>axis</i> : [Vector3](../objects/Vector3.md)<br/>)|float|Calculates the signed angle between vectors from and to in relation to axis.|
|Slerp(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md),<br/><i>t</i> : float<br/>)|[Vector3](../objects/Vector3.md)|Spherically interpolates between two vectors.|
|SlerpUnclamped(<br/><i>a</i> : [Vector3](../objects/Vector3.md),<br/><i>b</i> : [Vector3](../objects/Vector3.md),<br/><i>t</i> : float<br/>)|[Vector3](../objects/Vector3.md)|Spherically interpolates between two vectors.|
|SmoothDamp(<br/><i>current</i> : [Vector3](../objects/Vector3.md),<br/><i>target</i> : [Vector3](../objects/Vector3.md),<br/><i>currentVelocity</i> : [Vector3](../objects/Vector3.md),<br/><i>smoothTime</i> : float,<br/><i>maxSpeed</i> : float<br/>)|[Vector3](../objects/Vector3.md)||
