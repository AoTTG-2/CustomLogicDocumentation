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
|Function|Returns|Description|
|---|---|---|
|Set(<br/>x : float,<br/>y : float<br/>)|none|Set x and y components of an existing Vector2.|
|Normalize()|none|Makes this vector have a magnitude of 1.|
|\_\_Copy\_\_()|Object|Override to deepcopy object on assignment, used for structs. Ex: copy = original is equivalent to copy = original.\_\_Copy\_\_()|
|\_\_Add\_\_(<br/>self : Object,<br/>other : Object<br/>)|Object|Override to implement addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)|
|\_\_Sub\_\_(<br/>self : Object,<br/>other : Object<br/>)|Object|Override to implement subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)|
|\_\_Mul\_\_(<br/>self : Object,<br/>other : Object<br/>)|Object|Override to implement multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)|
|\_\_Div\_\_(<br/>self : Object,<br/>other : Object<br/>)|Object|Override to implement division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)|
|\_\_Eq\_\_(<br/>self : Object,<br/>other : Object<br/>)|bool|Override to implement equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)|
|\_\_Hash\_\_()|int|Override to implement hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()|
## Static Methods
|Function|Returns|Description|
|---|---|---|
|Angle(<br/>from : [Vector2](../objects/Vector2.md),<br/>to : [Vector2](../objects/Vector2.md)<br/>)|float|Gets the unsigned angle in degrees between from and to.|
|ClampMagnitude(<br/>vector : [Vector2](../objects/Vector2.md),<br/>maxLength : float<br/>)|[Vector2](../objects/Vector2.md)|Returns a copy of vector with its magnitude clamped to maxLength.|
|Distance(<br/>a : [Vector2](../objects/Vector2.md),<br/>b : [Vector2](../objects/Vector2.md)<br/>)|float|Returns the distance between a and b.|
|Dot(<br/>a : [Vector2](../objects/Vector2.md),<br/>b : [Vector2](../objects/Vector2.md)<br/>)|float|Dot Product of two vectors.|
|Lerp(<br/>a : [Vector2](../objects/Vector2.md),<br/>b : [Vector2](../objects/Vector2.md),<br/>t : float<br/>)|[Vector2](../objects/Vector2.md)|Linearly interpolates between vectors a and b by t.|
|LerpUnclamped(<br/>a : [Vector2](../objects/Vector2.md),<br/>b : [Vector2](../objects/Vector2.md),<br/>t : float<br/>)|[Vector2](../objects/Vector2.md)|Linearly interpolates between vectors a and b by t.|
|Max(<br/>a : [Vector2](../objects/Vector2.md),<br/>b : [Vector2](../objects/Vector2.md)<br/>)|[Vector2](../objects/Vector2.md)|Returns a vector that is made from the largest components of two vectors.|
|Min(<br/>a : [Vector2](../objects/Vector2.md),<br/>b : [Vector2](../objects/Vector2.md)<br/>)|[Vector2](../objects/Vector2.md)|Returns a vector that is made from the smallest components of two vectors.|
|MoveTowards(<br/>current : [Vector2](../objects/Vector2.md),<br/>target : [Vector2](../objects/Vector2.md),<br/>maxDistanceDelta : float<br/>)|[Vector2](../objects/Vector2.md)|Moves a point current towards target.|
|Reflect(<br/>inDirection : [Vector2](../objects/Vector2.md),<br/>inNormal : [Vector2](../objects/Vector2.md)<br/>)|[Vector2](../objects/Vector2.md)|Reflects a vector off the vector defined by a normal.|
|SignedAngle(<br/>from : [Vector2](../objects/Vector2.md),<br/>to : [Vector2](../objects/Vector2.md)<br/>)|float|Gets the signed angle in degrees between from and to.|
|SmoothDamp(<br/>current : [Vector2](../objects/Vector2.md),<br/>target : [Vector2](../objects/Vector2.md),<br/>currentVelocity : [Vector2](../objects/Vector2.md),<br/>smoothTime : float,<br/>maxSpeed : float<br/>)|[Vector2](../objects/Vector2.md)||
