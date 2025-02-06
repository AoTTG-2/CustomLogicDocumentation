# Math
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|PI|float|False|The value of PI|
|Infinity|float|False|The value of Infinity|
|NegativeInfinity|float|False|The value of Negative Infinity|
|Rad2DegConstant|float|False|The value of Rad2Deg constant|
|Deg2RadConstant|float|False|The value of Deg2Rad constant|
|Epsilon|float|False|The value of Epsilon|
## Methods
|Function|Returns|Description|
|---|---|---|
|Clamp(<br/>value : Object,<br/>min : Object,<br/>max : Object<br/>)|Object|Clamp a value between a minimum and maximum value|
|Max(<br/>a : Object,<br/>b : Object<br/>)|Object|Get the maximum of two values|
|Min(<br/>a : Object,<br/>b : Object<br/>)|Object|Get the minimum of two values|
|Pow(<br/>a : Object,<br/>b : Object<br/>)|Object|Raise a value to the power of another value|
|Abs(value : Object)|Object|Get the absolute value of a number|
|Sqrt(value : Object)|Object|Get the square root of a number|
|Mod(<br/>a : Object,<br/>b : Object<br/>)|Object|Get the remainder of a division operation|
|Sin(angle : Object)|Object|Get the sine of an angle in degrees|
|Cos(angle : Object)|Object|Get the cosine of an angle in degrees|
|Tan(angle : Object)|Object|Get the tangent of an angle in degrees|
|Asin(value : Object)|Object|Get the arcsine of a value in degrees|
|Acos(value : Object)|Object|Get the arccosine of a value in degrees|
|Atan(value : Object)|Object|Get the arctangent of a value in degrees|
|Atan2(<br/>a : Object,<br/>b : Object<br/>)|Object|Get the arctangent of a value in degrees|
|Ceil(value : Object)|Object|Get the smallest integer greater than or equal to a value|
|Floor(value : Object)|Object|Get the largest integer less than or equal to a value|
|Round(value : Object)|Object|Round a value to the nearest integer|
|Deg2Rad(angle : Object)|Object|Convert an angle from degrees to radians|
|Rad2Deg(angle : Object)|Object|Convert an angle from radians to degrees|
|Lerp(<br/>a : Object,<br/>b : Object,<br/>t : Object<br/>)|Object|Linearly interpolate between two values|
|LerpUnclamped(<br/>a : Object,<br/>b : Object,<br/>t : Object<br/>)|Object|Linearly interpolate between two values without clamping|
|Sign(value : Object)|Object|Get the sign of a value|
|InverseLerp(<br/>a : Object,<br/>b : Object,<br/>value : Object<br/>)|Object|Get the inverse lerp of two values|
|LerpAngle(<br/>a : Object,<br/>b : Object,<br/>t : Object<br/>)|Object|Linearly interpolate between two angles|
|Log(value : Object)|Object|Get the natural logarithm of a value|
|MoveTowards(<br/>current : Object,<br/>target : Object,<br/>maxDelta : Object<br/>)|Object|Move a value towards a target value|
|MoveTowardsAngle(<br/>current : Object,<br/>target : Object,<br/>maxDelta : Object<br/>)|Object|Move an angle towards a target angle|
|PingPong(<br/>t : Object,<br/>length : Object<br/>)|Object|Get the ping pong value of a time value|
|SmoothDamp(<br/>current : Object,<br/>target : Object,<br/>currentVelocity : Object,<br/>smoothTime : Object,<br/>maxSpeed : Object,<br/>deltaTime : Object<br/>)|Object|Smoothly damp a value towards a target value|
|Exp(value : Object)|Object|Get the exponential value of a number|
|SmoothDampAngle(<br/>current : Object,<br/>target : Object,<br/>currentVelocity : Object,<br/>smoothTime : Object,<br/>maxSpeed : Object,<br/>deltaTime : Object<br/>)|Object|Smoothly damp an angle towards a target angle|
|SmoothStep(<br/>a : Object,<br/>b : Object,<br/>t : Object<br/>)|Object|Smoothly step between two values|
|BitwiseAnd(<br/>a : Object,<br/>b : Object<br/>)|Object|Perform a bitwise AND operation|
|BitwiseOr(<br/>a : Object,<br/>b : Object<br/>)|Object|Perform a bitwise OR operation|
|BitwiseXor(<br/>a : Object,<br/>b : Object<br/>)|Object|Perform a bitwise XOR operation|
|BitwiseNot(value : Object)|Object|Perform a bitwise NOT operation|
|BitwiseLeftShift(<br/>value : Object,<br/>shift : Object<br/>)|Object|Shift bits to the left|
|BitwiseRightShift(<br/>value : Object,<br/>shift : Object<br/>)|Object|Shift bits to the right|
