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
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Clamp</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">min</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">max</mark>)
Clamp a value between a minimum and maximum value
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Max</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>)
Get the maximum of two values
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Min</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>)
Get the minimum of two values
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Pow</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>)
Raise a value to the power of another value
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Abs</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the absolute value of a number
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Sqrt</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the square root of a number
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Mod</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>)
Get the remainder of a division operation
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Sin</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">angle</mark>)
Get the sine of an angle in degrees
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Cos</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">angle</mark>)
Get the cosine of an angle in degrees
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Tan</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">angle</mark>)
Get the tangent of an angle in degrees
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Asin</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the arcsine of a value in degrees
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Acos</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the arccosine of a value in degrees
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Atan</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the arctangent of a value in degrees
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Atan2</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>)
Get the arctangent of a value in degrees
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Ceil</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the smallest integer greater than or equal to a value
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Floor</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the largest integer less than or equal to a value
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Round</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Round a value to the nearest integer
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Deg2Rad</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">angle</mark>)
Convert an angle from degrees to radians
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Rad2Deg</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">angle</mark>)
Convert an angle from radians to degrees
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Lerp</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">t</mark>)
Linearly interpolate between two values
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">LerpUnclamped</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">t</mark>)
Linearly interpolate between two values without clamping
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Sign</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the sign of a value
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">InverseLerp</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the inverse lerp of two values
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">LerpAngle</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">t</mark>)
Linearly interpolate between two angles
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Log</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the natural logarithm of a value
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">MoveTowards</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">current</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">maxDelta</mark>)
Move a value towards a target value
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">MoveTowardsAngle</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">current</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">maxDelta</mark>)
Move an angle towards a target angle
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">PingPong</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">t</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">length</mark>)
Get the ping pong value of a time value
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">SmoothDamp</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">current</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">currentVelocity</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">smoothTime</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">maxSpeed</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">deltaTime</mark>)
Smoothly damp a value towards a target value
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">Exp</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Get the exponential value of a number
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">SmoothDampAngle</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">current</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">currentVelocity</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">smoothTime</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">maxSpeed</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">deltaTime</mark>)
Smoothly damp an angle towards a target angle
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">SmoothStep</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">t</mark>)
Smoothly step between two values
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">BitwiseAnd</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>)
Perform a bitwise AND operation
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">BitwiseOr</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>)
Perform a bitwise OR operation
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">BitwiseXor</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">a</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">b</mark>)
Perform a bitwise XOR operation
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">BitwiseNot</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Perform a bitwise NOT operation
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">BitwiseLeftShift</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">shift</mark>)
Shift bits to the left
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">BitwiseRightShift</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">shift</mark>)
Shift bits to the right

---

