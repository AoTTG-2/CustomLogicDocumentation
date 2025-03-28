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
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Clamp</mark>(<mark style="color:blue;">Object</mark> value, <mark style="color:blue;">Object</mark> min, <mark style="color:blue;">Object</mark> max)
> Clamp a value between a minimum and maximum value

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Max</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b)
> Get the maximum of two values

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Min</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b)
> Get the minimum of two values

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Pow</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b)
> Raise a value to the power of another value

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Abs</mark>(<mark style="color:blue;">Object</mark> value)
> Get the absolute value of a number

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Sqrt</mark>(<mark style="color:blue;">Object</mark> value)
> Get the square root of a number

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Mod</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b)
> Get the remainder of a division operation

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Sin</mark>(<mark style="color:blue;">Object</mark> angle)
> Get the sine of an angle in degrees

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Cos</mark>(<mark style="color:blue;">Object</mark> angle)
> Get the cosine of an angle in degrees

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Tan</mark>(<mark style="color:blue;">Object</mark> angle)
> Get the tangent of an angle in degrees

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Asin</mark>(<mark style="color:blue;">Object</mark> value)
> Get the arcsine of a value in degrees

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Acos</mark>(<mark style="color:blue;">Object</mark> value)
> Get the arccosine of a value in degrees

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Atan</mark>(<mark style="color:blue;">Object</mark> value)
> Get the arctangent of a value in degrees

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Atan2</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b)
> Get the arctangent of a value in degrees

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Ceil</mark>(<mark style="color:blue;">Object</mark> value)
> Get the smallest integer greater than or equal to a value

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Floor</mark>(<mark style="color:blue;">Object</mark> value)
> Get the largest integer less than or equal to a value

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Round</mark>(<mark style="color:blue;">Object</mark> value)
> Round a value to the nearest integer

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Deg2Rad</mark>(<mark style="color:blue;">Object</mark> angle)
> Convert an angle from degrees to radians

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Rad2Deg</mark>(<mark style="color:blue;">Object</mark> angle)
> Convert an angle from radians to degrees

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Lerp</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b, <mark style="color:blue;">Object</mark> t)
> Linearly interpolate between two values

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">LerpUnclamped</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b, <mark style="color:blue;">Object</mark> t)
> Linearly interpolate between two values without clamping

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Sign</mark>(<mark style="color:blue;">Object</mark> value)
> Get the sign of a value

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">InverseLerp</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b, <mark style="color:blue;">Object</mark> value)
> Get the inverse lerp of two values

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">LerpAngle</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b, <mark style="color:blue;">Object</mark> t)
> Linearly interpolate between two angles

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Log</mark>(<mark style="color:blue;">Object</mark> value)
> Get the natural logarithm of a value

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">MoveTowards</mark>(<mark style="color:blue;">Object</mark> current, <mark style="color:blue;">Object</mark> target, <mark style="color:blue;">Object</mark> maxDelta)
> Move a value towards a target value

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">MoveTowardsAngle</mark>(<mark style="color:blue;">Object</mark> current, <mark style="color:blue;">Object</mark> target, <mark style="color:blue;">Object</mark> maxDelta)
> Move an angle towards a target angle

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">PingPong</mark>(<mark style="color:blue;">Object</mark> t, <mark style="color:blue;">Object</mark> length)
> Get the ping pong value of a time value

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">SmoothDamp</mark>(<mark style="color:blue;">Object</mark> current, <mark style="color:blue;">Object</mark> target, <mark style="color:blue;">Object</mark> currentVelocity, <mark style="color:blue;">Object</mark> smoothTime, <mark style="color:blue;">Object</mark> maxSpeed, <mark style="color:blue;">Object</mark> deltaTime)
> Smoothly damp a value towards a target value

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">Exp</mark>(<mark style="color:blue;">Object</mark> value)
> Get the exponential value of a number

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">SmoothDampAngle</mark>(<mark style="color:blue;">Object</mark> current, <mark style="color:blue;">Object</mark> target, <mark style="color:blue;">Object</mark> currentVelocity, <mark style="color:blue;">Object</mark> smoothTime, <mark style="color:blue;">Object</mark> maxSpeed, <mark style="color:blue;">Object</mark> deltaTime)
> Smoothly damp an angle towards a target angle

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">SmoothStep</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b, <mark style="color:blue;">Object</mark> t)
> Smoothly step between two values

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseAnd</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b)
> Perform a bitwise AND operation

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseOr</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b)
> Perform a bitwise OR operation

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseXor</mark>(<mark style="color:blue;">Object</mark> a, <mark style="color:blue;">Object</mark> b)
> Perform a bitwise XOR operation

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseNot</mark>(<mark style="color:blue;">Object</mark> value)
> Perform a bitwise NOT operation

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseLeftShift</mark>(<mark style="color:blue;">Object</mark> value, <mark style="color:blue;">Object</mark> shift)
> Shift bits to the left

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">BitwiseRightShift</mark>(<mark style="color:blue;">Object</mark> value, <mark style="color:blue;">Object</mark> shift)
> Shift bits to the right


---

