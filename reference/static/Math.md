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
#### Object <span style="color":#dcdcaa>Clamp<span>(Object <span style="color":#9cdcfe>value<span>, Object <span style="color":#9cdcfe>min<span>, Object <span style="color":#9cdcfe>max<span>)
Clamp a value between a minimum and maximum value
#### Object <span style="color":#dcdcaa>Max<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>)
Get the maximum of two values
#### Object <span style="color":#dcdcaa>Min<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>)
Get the minimum of two values
#### Object <span style="color":#dcdcaa>Pow<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>)
Raise a value to the power of another value
#### Object <span style="color":#dcdcaa>Abs<span>(Object <span style="color":#9cdcfe>value<span>)
Get the absolute value of a number
#### Object <span style="color":#dcdcaa>Sqrt<span>(Object <span style="color":#9cdcfe>value<span>)
Get the square root of a number
#### Object <span style="color":#dcdcaa>Mod<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>)
Get the remainder of a division operation
#### Object <span style="color":#dcdcaa>Sin<span>(Object <span style="color":#9cdcfe>angle<span>)
Get the sine of an angle in degrees
#### Object <span style="color":#dcdcaa>Cos<span>(Object <span style="color":#9cdcfe>angle<span>)
Get the cosine of an angle in degrees
#### Object <span style="color":#dcdcaa>Tan<span>(Object <span style="color":#9cdcfe>angle<span>)
Get the tangent of an angle in degrees
#### Object <span style="color":#dcdcaa>Asin<span>(Object <span style="color":#9cdcfe>value<span>)
Get the arcsine of a value in degrees
#### Object <span style="color":#dcdcaa>Acos<span>(Object <span style="color":#9cdcfe>value<span>)
Get the arccosine of a value in degrees
#### Object <span style="color":#dcdcaa>Atan<span>(Object <span style="color":#9cdcfe>value<span>)
Get the arctangent of a value in degrees
#### Object <span style="color":#dcdcaa>Atan2<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>)
Get the arctangent of a value in degrees
#### Object <span style="color":#dcdcaa>Ceil<span>(Object <span style="color":#9cdcfe>value<span>)
Get the smallest integer greater than or equal to a value
#### Object <span style="color":#dcdcaa>Floor<span>(Object <span style="color":#9cdcfe>value<span>)
Get the largest integer less than or equal to a value
#### Object <span style="color":#dcdcaa>Round<span>(Object <span style="color":#9cdcfe>value<span>)
Round a value to the nearest integer
#### Object <span style="color":#dcdcaa>Deg2Rad<span>(Object <span style="color":#9cdcfe>angle<span>)
Convert an angle from degrees to radians
#### Object <span style="color":#dcdcaa>Rad2Deg<span>(Object <span style="color":#9cdcfe>angle<span>)
Convert an angle from radians to degrees
#### Object <span style="color":#dcdcaa>Lerp<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>, Object <span style="color":#9cdcfe>t<span>)
Linearly interpolate between two values
#### Object <span style="color":#dcdcaa>LerpUnclamped<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>, Object <span style="color":#9cdcfe>t<span>)
Linearly interpolate between two values without clamping
#### Object <span style="color":#dcdcaa>Sign<span>(Object <span style="color":#9cdcfe>value<span>)
Get the sign of a value
#### Object <span style="color":#dcdcaa>InverseLerp<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>, Object <span style="color":#9cdcfe>value<span>)
Get the inverse lerp of two values
#### Object <span style="color":#dcdcaa>LerpAngle<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>, Object <span style="color":#9cdcfe>t<span>)
Linearly interpolate between two angles
#### Object <span style="color":#dcdcaa>Log<span>(Object <span style="color":#9cdcfe>value<span>)
Get the natural logarithm of a value
#### Object <span style="color":#dcdcaa>MoveTowards<span>(Object <span style="color":#9cdcfe>current<span>, Object <span style="color":#9cdcfe>target<span>, Object <span style="color":#9cdcfe>maxDelta<span>)
Move a value towards a target value
#### Object <span style="color":#dcdcaa>MoveTowardsAngle<span>(Object <span style="color":#9cdcfe>current<span>, Object <span style="color":#9cdcfe>target<span>, Object <span style="color":#9cdcfe>maxDelta<span>)
Move an angle towards a target angle
#### Object <span style="color":#dcdcaa>PingPong<span>(Object <span style="color":#9cdcfe>t<span>, Object <span style="color":#9cdcfe>length<span>)
Get the ping pong value of a time value
#### Object <span style="color":#dcdcaa>SmoothDamp<span>(Object <span style="color":#9cdcfe>current<span>, Object <span style="color":#9cdcfe>target<span>, Object <span style="color":#9cdcfe>currentVelocity<span>, Object <span style="color":#9cdcfe>smoothTime<span>, Object <span style="color":#9cdcfe>maxSpeed<span>, Object <span style="color":#9cdcfe>deltaTime<span>)
Smoothly damp a value towards a target value
#### Object <span style="color":#dcdcaa>Exp<span>(Object <span style="color":#9cdcfe>value<span>)
Get the exponential value of a number
#### Object <span style="color":#dcdcaa>SmoothDampAngle<span>(Object <span style="color":#9cdcfe>current<span>, Object <span style="color":#9cdcfe>target<span>, Object <span style="color":#9cdcfe>currentVelocity<span>, Object <span style="color":#9cdcfe>smoothTime<span>, Object <span style="color":#9cdcfe>maxSpeed<span>, Object <span style="color":#9cdcfe>deltaTime<span>)
Smoothly damp an angle towards a target angle
#### Object <span style="color":#dcdcaa>SmoothStep<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>, Object <span style="color":#9cdcfe>t<span>)
Smoothly step between two values
#### Object <span style="color":#dcdcaa>BitwiseAnd<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>)
Perform a bitwise AND operation
#### Object <span style="color":#dcdcaa>BitwiseOr<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>)
Perform a bitwise OR operation
#### Object <span style="color":#dcdcaa>BitwiseXor<span>(Object <span style="color":#9cdcfe>a<span>, Object <span style="color":#9cdcfe>b<span>)
Perform a bitwise XOR operation
#### Object <span style="color":#dcdcaa>BitwiseNot<span>(Object <span style="color":#9cdcfe>value<span>)
Perform a bitwise NOT operation
#### Object <span style="color":#dcdcaa>BitwiseLeftShift<span>(Object <span style="color":#9cdcfe>value<span>, Object <span style="color":#9cdcfe>shift<span>)
Shift bits to the left
#### Object <span style="color":#dcdcaa>BitwiseRightShift<span>(Object <span style="color":#9cdcfe>value<span>, Object <span style="color":#9cdcfe>shift<span>)
Shift bits to the right

---

