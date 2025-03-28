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
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Clamp</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">min</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">max</mark>)
Clamp a value between a minimum and maximum value
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Max</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>)
Get the maximum of two values
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Min</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>)
Get the minimum of two values
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Pow</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>)
Raise a value to the power of another value
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Abs</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the absolute value of a number
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Sqrt</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the square root of a number
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Mod</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>)
Get the remainder of a division operation
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Sin</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">angle</mark>)
Get the sine of an angle in degrees
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Cos</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">angle</mark>)
Get the cosine of an angle in degrees
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Tan</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">angle</mark>)
Get the tangent of an angle in degrees
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Asin</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the arcsine of a value in degrees
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Acos</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the arccosine of a value in degrees
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Atan</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the arctangent of a value in degrees
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Atan2</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>)
Get the arctangent of a value in degrees
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Ceil</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the smallest integer greater than or equal to a value
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Floor</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the largest integer less than or equal to a value
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Round</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Round a value to the nearest integer
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Deg2Rad</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">angle</mark>)
Convert an angle from degrees to radians
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Rad2Deg</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">angle</mark>)
Convert an angle from radians to degrees
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Lerp</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">t</mark>)
Linearly interpolate between two values
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">LerpUnclamped</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">t</mark>)
Linearly interpolate between two values without clamping
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Sign</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the sign of a value
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">InverseLerp</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the inverse lerp of two values
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">LerpAngle</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">t</mark>)
Linearly interpolate between two angles
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Log</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the natural logarithm of a value
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">MoveTowards</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">current</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">maxDelta</mark>)
Move a value towards a target value
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">MoveTowardsAngle</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">current</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">maxDelta</mark>)
Move an angle towards a target angle
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">PingPong</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">t</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">length</mark>)
Get the ping pong value of a time value
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">SmoothDamp</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">current</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">currentVelocity</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">smoothTime</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">maxSpeed</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">deltaTime</mark>)
Smoothly damp a value towards a target value
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Exp</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Get the exponential value of a number
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">SmoothDampAngle</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">current</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">currentVelocity</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">smoothTime</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">maxSpeed</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">deltaTime</mark>)
Smoothly damp an angle towards a target angle
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">SmoothStep</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">t</mark>)
Smoothly step between two values
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseAnd</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>)
Perform a bitwise AND operation
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseOr</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>)
Perform a bitwise OR operation
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseXor</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">a</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">b</mark>)
Perform a bitwise XOR operation
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseNot</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>)
Perform a bitwise NOT operation
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseLeftShift</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">shift</mark>)
Shift bits to the left
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseRightShift</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">value</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">shift</mark>)
Shift bits to the right

---

