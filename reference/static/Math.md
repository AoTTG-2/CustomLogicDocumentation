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
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Clamp</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">min</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">max</mark>)
Clamp a value between a minimum and maximum value
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Max</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>)
Get the maximum of two values
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Min</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>)
Get the minimum of two values
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Pow</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>)
Raise a value to the power of another value
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Abs</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the absolute value of a number
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Sqrt</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the square root of a number
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Mod</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>)
Get the remainder of a division operation
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Sin</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">angle</mark>)
Get the sine of an angle in degrees
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Cos</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">angle</mark>)
Get the cosine of an angle in degrees
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Tan</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">angle</mark>)
Get the tangent of an angle in degrees
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Asin</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the arcsine of a value in degrees
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Acos</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the arccosine of a value in degrees
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Atan</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the arctangent of a value in degrees
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Atan2</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>)
Get the arctangent of a value in degrees
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Ceil</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the smallest integer greater than or equal to a value
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Floor</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the largest integer less than or equal to a value
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Round</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Round a value to the nearest integer
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Deg2Rad</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">angle</mark>)
Convert an angle from degrees to radians
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Rad2Deg</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">angle</mark>)
Convert an angle from radians to degrees
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Lerp</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">t</mark>)
Linearly interpolate between two values
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">LerpUnclamped</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">t</mark>)
Linearly interpolate between two values without clamping
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Sign</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the sign of a value
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">InverseLerp</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the inverse lerp of two values
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">LerpAngle</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">t</mark>)
Linearly interpolate between two angles
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Log</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the natural logarithm of a value
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">MoveTowards</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">current</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">target</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">maxDelta</mark>)
Move a value towards a target value
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">MoveTowardsAngle</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">current</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">target</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">maxDelta</mark>)
Move an angle towards a target angle
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">PingPong</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">t</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">length</mark>)
Get the ping pong value of a time value
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">SmoothDamp</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">current</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">target</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">currentVelocity</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">smoothTime</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">maxSpeed</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">deltaTime</mark>)
Smoothly damp a value towards a target value
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">Exp</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Get the exponential value of a number
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">SmoothDampAngle</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">current</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">target</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">currentVelocity</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">smoothTime</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">maxSpeed</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">deltaTime</mark>)
Smoothly damp an angle towards a target angle
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">SmoothStep</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">t</mark>)
Smoothly step between two values
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">BitwiseAnd</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>)
Perform a bitwise AND operation
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">BitwiseOr</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>)
Perform a bitwise OR operation
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">BitwiseXor</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">a</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">b</mark>)
Perform a bitwise XOR operation
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">BitwiseNot</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Perform a bitwise NOT operation
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">BitwiseLeftShift</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">shift</mark>)
Shift bits to the left
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">BitwiseRightShift</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">shift</mark>)
Shift bits to the right

---

