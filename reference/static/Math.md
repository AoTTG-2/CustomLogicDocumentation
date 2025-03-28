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
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Clamp</span>(<span style="color:blue;">Object</span> value, <span style="color:blue;">Object</span> min, <span style="color:blue;">Object</span> max)
> Clamp a value between a minimum and maximum value
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Max</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b)
> Get the maximum of two values
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Min</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b)
> Get the minimum of two values
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Pow</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b)
> Raise a value to the power of another value
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Abs</span>(<span style="color:blue;">Object</span> value)
> Get the absolute value of a number
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Sqrt</span>(<span style="color:blue;">Object</span> value)
> Get the square root of a number
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Mod</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b)
> Get the remainder of a division operation
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Sin</span>(<span style="color:blue;">Object</span> angle)
> Get the sine of an angle in degrees
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Cos</span>(<span style="color:blue;">Object</span> angle)
> Get the cosine of an angle in degrees
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Tan</span>(<span style="color:blue;">Object</span> angle)
> Get the tangent of an angle in degrees
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Asin</span>(<span style="color:blue;">Object</span> value)
> Get the arcsine of a value in degrees
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Acos</span>(<span style="color:blue;">Object</span> value)
> Get the arccosine of a value in degrees
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Atan</span>(<span style="color:blue;">Object</span> value)
> Get the arctangent of a value in degrees
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Atan2</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b)
> Get the arctangent of a value in degrees
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Ceil</span>(<span style="color:blue;">Object</span> value)
> Get the smallest integer greater than or equal to a value
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Floor</span>(<span style="color:blue;">Object</span> value)
> Get the largest integer less than or equal to a value
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Round</span>(<span style="color:blue;">Object</span> value)
> Round a value to the nearest integer
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Deg2Rad</span>(<span style="color:blue;">Object</span> angle)
> Convert an angle from degrees to radians
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Rad2Deg</span>(<span style="color:blue;">Object</span> angle)
> Convert an angle from radians to degrees
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Lerp</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b, <span style="color:blue;">Object</span> t)
> Linearly interpolate between two values
#### <span style="color:blue;">Object</span> <span style="color:yellow;">LerpUnclamped</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b, <span style="color:blue;">Object</span> t)
> Linearly interpolate between two values without clamping
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Sign</span>(<span style="color:blue;">Object</span> value)
> Get the sign of a value
#### <span style="color:blue;">Object</span> <span style="color:yellow;">InverseLerp</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b, <span style="color:blue;">Object</span> value)
> Get the inverse lerp of two values
#### <span style="color:blue;">Object</span> <span style="color:yellow;">LerpAngle</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b, <span style="color:blue;">Object</span> t)
> Linearly interpolate between two angles
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Log</span>(<span style="color:blue;">Object</span> value)
> Get the natural logarithm of a value
#### <span style="color:blue;">Object</span> <span style="color:yellow;">MoveTowards</span>(<span style="color:blue;">Object</span> current, <span style="color:blue;">Object</span> target, <span style="color:blue;">Object</span> maxDelta)
> Move a value towards a target value
#### <span style="color:blue;">Object</span> <span style="color:yellow;">MoveTowardsAngle</span>(<span style="color:blue;">Object</span> current, <span style="color:blue;">Object</span> target, <span style="color:blue;">Object</span> maxDelta)
> Move an angle towards a target angle
#### <span style="color:blue;">Object</span> <span style="color:yellow;">PingPong</span>(<span style="color:blue;">Object</span> t, <span style="color:blue;">Object</span> length)
> Get the ping pong value of a time value
#### <span style="color:blue;">Object</span> <span style="color:yellow;">SmoothDamp</span>(<span style="color:blue;">Object</span> current, <span style="color:blue;">Object</span> target, <span style="color:blue;">Object</span> currentVelocity, <span style="color:blue;">Object</span> smoothTime, <span style="color:blue;">Object</span> maxSpeed, <span style="color:blue;">Object</span> deltaTime)
> Smoothly damp a value towards a target value
#### <span style="color:blue;">Object</span> <span style="color:yellow;">Exp</span>(<span style="color:blue;">Object</span> value)
> Get the exponential value of a number
#### <span style="color:blue;">Object</span> <span style="color:yellow;">SmoothDampAngle</span>(<span style="color:blue;">Object</span> current, <span style="color:blue;">Object</span> target, <span style="color:blue;">Object</span> currentVelocity, <span style="color:blue;">Object</span> smoothTime, <span style="color:blue;">Object</span> maxSpeed, <span style="color:blue;">Object</span> deltaTime)
> Smoothly damp an angle towards a target angle
#### <span style="color:blue;">Object</span> <span style="color:yellow;">SmoothStep</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b, <span style="color:blue;">Object</span> t)
> Smoothly step between two values
#### <span style="color:blue;">Object</span> <span style="color:yellow;">BitwiseAnd</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b)
> Perform a bitwise AND operation
#### <span style="color:blue;">Object</span> <span style="color:yellow;">BitwiseOr</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b)
> Perform a bitwise OR operation
#### <span style="color:blue;">Object</span> <span style="color:yellow;">BitwiseXor</span>(<span style="color:blue;">Object</span> a, <span style="color:blue;">Object</span> b)
> Perform a bitwise XOR operation
#### <span style="color:blue;">Object</span> <span style="color:yellow;">BitwiseNot</span>(<span style="color:blue;">Object</span> value)
> Perform a bitwise NOT operation
#### <span style="color:blue;">Object</span> <span style="color:yellow;">BitwiseLeftShift</span>(<span style="color:blue;">Object</span> value, <span style="color:blue;">Object</span> shift)
> Shift bits to the left
#### <span style="color:blue;">Object</span> <span style="color:yellow;">BitwiseRightShift</span>(<span style="color:blue;">Object</span> value, <span style="color:blue;">Object</span> shift)
> Shift bits to the right

---

