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
|Clamp(<br/><i>value</i> : Object,<br/><i>min</i> : Object,<br/><i>max</i> : Object<br/>)|Object|Clamp a value between a minimum and maximum value|
|Max(<br/><i>a</i> : Object,<br/><i>b</i> : Object<br/>)|Object|Get the maximum of two values|
|Min(<br/><i>a</i> : Object,<br/><i>b</i> : Object<br/>)|Object|Get the minimum of two values|
|Pow(<br/><i>a</i> : Object,<br/><i>b</i> : Object<br/>)|Object|Raise a value to the power of another value|
|Abs(<i>value</i> : Object)|Object|Get the absolute value of a number|
|Sqrt(<i>value</i> : Object)|Object|Get the square root of a number|
|Mod(<br/><i>a</i> : Object,<br/><i>b</i> : Object<br/>)|Object|Get the remainder of a division operation|
|Sin(<i>angle</i> : Object)|Object|Get the sine of an angle in degrees|
|Cos(<i>angle</i> : Object)|Object|Get the cosine of an angle in degrees|
|Tan(<i>angle</i> : Object)|Object|Get the tangent of an angle in degrees|
|Asin(<i>value</i> : Object)|Object|Get the arcsine of a value in degrees|
|Acos(<i>value</i> : Object)|Object|Get the arccosine of a value in degrees|
|Atan(<i>value</i> : Object)|Object|Get the arctangent of a value in degrees|
|Atan2(<br/><i>a</i> : Object,<br/><i>b</i> : Object<br/>)|Object|Get the arctangent of a value in degrees|
|Ceil(<i>value</i> : Object)|Object|Get the smallest integer greater than or equal to a value|
|Floor(<i>value</i> : Object)|Object|Get the largest integer less than or equal to a value|
|Round(<i>value</i> : Object)|Object|Round a value to the nearest integer|
|Deg2Rad(<i>angle</i> : Object)|Object|Convert an angle from degrees to radians|
|Rad2Deg(<i>angle</i> : Object)|Object|Convert an angle from radians to degrees|
|Lerp(<br/><i>a</i> : Object,<br/><i>b</i> : Object,<br/><i>t</i> : Object<br/>)|Object|Linearly interpolate between two values|
|LerpUnclamped(<br/><i>a</i> : Object,<br/><i>b</i> : Object,<br/><i>t</i> : Object<br/>)|Object|Linearly interpolate between two values without clamping|
|Sign(<i>value</i> : Object)|Object|Get the sign of a value|
|InverseLerp(<br/><i>a</i> : Object,<br/><i>b</i> : Object,<br/><i>value</i> : Object<br/>)|Object|Get the inverse lerp of two values|
|LerpAngle(<br/><i>a</i> : Object,<br/><i>b</i> : Object,<br/><i>t</i> : Object<br/>)|Object|Linearly interpolate between two angles|
|Log(<i>value</i> : Object)|Object|Get the natural logarithm of a value|
|MoveTowards(<br/><i>current</i> : Object,<br/><i>target</i> : Object,<br/><i>maxDelta</i> : Object<br/>)|Object|Move a value towards a target value|
|MoveTowardsAngle(<br/><i>current</i> : Object,<br/><i>target</i> : Object,<br/><i>maxDelta</i> : Object<br/>)|Object|Move an angle towards a target angle|
|PingPong(<br/><i>t</i> : Object,<br/><i>length</i> : Object<br/>)|Object|Get the ping pong value of a time value|
|SmoothDamp(<br/><i>current</i> : Object,<br/><i>target</i> : Object,<br/><i>currentVelocity</i> : Object,<br/><i>smoothTime</i> : Object,<br/><i>maxSpeed</i> : Object,<br/><i>deltaTime</i> : Object<br/>)|Object|Smoothly damp a value towards a target value|
|Exp(<i>value</i> : Object)|Object|Get the exponential value of a number|
|SmoothDampAngle(<br/><i>current</i> : Object,<br/><i>target</i> : Object,<br/><i>currentVelocity</i> : Object,<br/><i>smoothTime</i> : Object,<br/><i>maxSpeed</i> : Object,<br/><i>deltaTime</i> : Object<br/>)|Object|Smoothly damp an angle towards a target angle|
|SmoothStep(<br/><i>a</i> : Object,<br/><i>b</i> : Object,<br/><i>t</i> : Object<br/>)|Object|Smoothly step between two values|
|BitwiseAnd(<br/><i>a</i> : Object,<br/><i>b</i> : Object<br/>)|Object|Perform a bitwise AND operation|
|BitwiseOr(<br/><i>a</i> : Object,<br/><i>b</i> : Object<br/>)|Object|Perform a bitwise OR operation|
|BitwiseXor(<br/><i>a</i> : Object,<br/><i>b</i> : Object<br/>)|Object|Perform a bitwise XOR operation|
|BitwiseNot(<i>value</i> : Object)|Object|Perform a bitwise NOT operation|
|BitwiseLeftShift(<br/><i>value</i> : Object,<br/><i>shift</i> : Object<br/>)|Object|Shift bits to the left|
|BitwiseRightShift(<br/><i>value</i> : Object,<br/><i>shift</i> : Object<br/>)|Object|Shift bits to the right|
