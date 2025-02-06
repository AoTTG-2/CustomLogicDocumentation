# Vector3
Inherits from object
## Fields
|<div style="width:30%">Field</div>|<div style="width:5%">Type</div>|<div style="width:5%">Readonly</div>|<div style="width:60%">Description</div>|
|---|---|---|---|
|X|float|False|X component of the vector.|
|Y|float|False|Y component of the vector.|
|Z|float|False|Z component of the vector.|
|Normalized|[Vector3](../objects/Vector3.md)|False|Returns this vector with a magnitude of 1 (Read Only).|
|Magnitude|float|False|Returns the length of this vector (Read Only).|
|SqrMagnitude|float|False|Returns the squared length of this vector (Read Only).|
## Static Fields
|<div style="width:30%">Field</div>|<div style="width:5%">Type</div>|<div style="width:5%">Readonly</div>|<div style="width:60%">Description</div>|
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
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|Set(x : float,<br/>y : float,<br/>z : float)|none|Set x, y and z components of an existing Vector3.|
|Scale(scale : Object)|[Vector3](../objects/Vector3.md)|Returns the Vector3 multiplied by scale.|
|Multiply(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Returns the multiplication of two Vector3s.|
|Divide(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Returns the division of two Vector3s.|
|GetRotationDirection(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Gets the relational Vector3 "b" using "a" as a reference. This is equivalent to setting MapObject.Forward to Vector "a", and finding the relative "b" vector.|
|\_\_Copy\_\_()|Object|Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()|
|\_\_Add\_\_(self : Object,<br/>other : Object)|Object|Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)|
|\_\_Sub\_\_(self : Object,<br/>other : Object)|Object|Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)|
|\_\_Mul\_\_(self : Object,<br/>other : Object)|Object|Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)|
|\_\_Div\_\_(self : Object,<br/>other : Object)|Object|Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)|
|\_\_Eq\_\_(self : Object,<br/>other : Object)|bool|Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)|
|\_\_Hash\_\_()|int|Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()|
## Static Methods
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|Angle(from : [Vector3](../objects/Vector3.md),<br/>to : [Vector3](../objects/Vector3.md))|float|Calculates the angle between vectors from and.|
|ClampMagnitude(vector : [Vector3](../objects/Vector3.md),<br/>maxLength : float)|[Vector3](../objects/Vector3.md)|Returns a copy of vector with its magnitude clamped to maxLength.|
|Cross(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Cross Product of two vectors.|
|Distance(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|float|Returns the distance between a and b.|
|Dot(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|float|Dot Product of two vectors.|
|Lerp(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md),<br/>t : float)|[Vector3](../objects/Vector3.md)|Linearly interpolates between two points.|
|LerpUnclamped(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md),<br/>t : float)|[Vector3](../objects/Vector3.md)|Linearly interpolates between two vectors.|
|Max(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Returns a vector that is made from the largest components of two vectors.|
|Min(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Returns a vector that is made from the smallest components of two vectors.|
|MoveTowards(current : [Vector3](../objects/Vector3.md),<br/>target : [Vector3](../objects/Vector3.md),<br/>maxDistanceDelta : float)|[Vector3](../objects/Vector3.md)|Calculate a position between the points specified by current and target, moving no farther than the distance specified by maxDistanceDelta.|
|Normalize(value : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Makes this vector have a magnitude of 1.|
|OrthoNormalize(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|none||
|Project(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Projects a vector onto another vector.|
|ProjectOnPlane(vector : [Vector3](../objects/Vector3.md),<br/>plane : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Projects a vector onto a plane defined by a normal orthogonal to the plane.|
|Reflect(inDirection : [Vector3](../objects/Vector3.md),<br/>inNormal : [Vector3](../objects/Vector3.md))|[Vector3](../objects/Vector3.md)|Reflects a vector off the plane defined by a normal.|
|RotateTowards(current : [Vector3](../objects/Vector3.md),<br/>target : [Vector3](../objects/Vector3.md),<br/>maxRadiansDelta : float,<br/>maxMagnitudeDelta : float)|[Vector3](../objects/Vector3.md)|Rotates a vector current towards target.|
|SignedAngle(from : [Vector3](../objects/Vector3.md),<br/>to : [Vector3](../objects/Vector3.md),<br/>axis : [Vector3](../objects/Vector3.md))|float|Calculates the signed angle between vectors from and to in relation to axis.|
|Slerp(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md),<br/>t : float)|[Vector3](../objects/Vector3.md)|Spherically interpolates between two vectors.|
|SlerpUnclamped(a : [Vector3](../objects/Vector3.md),<br/>b : [Vector3](../objects/Vector3.md),<br/>t : float)|[Vector3](../objects/Vector3.md)|Spherically interpolates between two vectors.|
|SmoothDamp(current : [Vector3](../objects/Vector3.md),<br/>target : [Vector3](../objects/Vector3.md),<br/>currentVelocity : [Vector3](../objects/Vector3.md),<br/>smoothTime : float,<br/>maxSpeed : float)|[Vector3](../objects/Vector3.md)||
