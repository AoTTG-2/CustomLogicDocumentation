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
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Clamp</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">min</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">max</span>)
Clamp a value between a minimum and maximum value
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Max</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>)
Get the maximum of two values
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Min</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>)
Get the minimum of two values
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Pow</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>)
Raise a value to the power of another value
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Abs</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the absolute value of a number
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Sqrt</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the square root of a number
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Mod</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>)
Get the remainder of a division operation
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Sin</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">angle</span>)
Get the sine of an angle in degrees
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Cos</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">angle</span>)
Get the cosine of an angle in degrees
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Tan</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">angle</span>)
Get the tangent of an angle in degrees
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Asin</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the arcsine of a value in degrees
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Acos</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the arccosine of a value in degrees
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Atan</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the arctangent of a value in degrees
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Atan2</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>)
Get the arctangent of a value in degrees
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Ceil</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the smallest integer greater than or equal to a value
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Floor</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the largest integer less than or equal to a value
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Round</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Round a value to the nearest integer
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Deg2Rad</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">angle</span>)
Convert an angle from degrees to radians
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Rad2Deg</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">angle</span>)
Convert an angle from radians to degrees
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Lerp</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">t</span>)
Linearly interpolate between two values
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">LerpUnclamped</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">t</span>)
Linearly interpolate between two values without clamping
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Sign</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the sign of a value
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">InverseLerp</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the inverse lerp of two values
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">LerpAngle</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">t</span>)
Linearly interpolate between two angles
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Log</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the natural logarithm of a value
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">MoveTowards</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">current</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">target</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">maxDelta</span>)
Move a value towards a target value
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">MoveTowardsAngle</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">current</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">target</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">maxDelta</span>)
Move an angle towards a target angle
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">PingPong</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">t</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">length</span>)
Get the ping pong value of a time value
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">SmoothDamp</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">current</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">target</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">currentVelocity</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">smoothTime</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">maxSpeed</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">deltaTime</span>)
Smoothly damp a value towards a target value
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">Exp</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Get the exponential value of a number
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">SmoothDampAngle</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">current</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">target</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">currentVelocity</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">smoothTime</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">maxSpeed</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">deltaTime</span>)
Smoothly damp an angle towards a target angle
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">SmoothStep</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">t</span>)
Smoothly step between two values
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">BitwiseAnd</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>)
Perform a bitwise AND operation
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">BitwiseOr</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>)
Perform a bitwise OR operation
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">BitwiseXor</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">a</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">b</span>)
Perform a bitwise XOR operation
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">BitwiseNot</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>)
Perform a bitwise NOT operation
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">BitwiseLeftShift</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">shift</span>)
Shift bits to the left
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">BitwiseRightShift</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">value</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">shift</span>)
Shift bits to the right

---

