# Math
Inherits from [Object](../objects/Object.md)
### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|PI|float|True|The value of PI.|
|Infinity|float|True|The value of Infinity.|
|NegativeInfinity|float|True|The value of Negative Infinity.|
|Rad2DegConstant|float|True|The value of Rad2Deg constant.|
|Deg2RadConstant|float|True|The value of Deg2Rad constant.|
|Epsilon|float|True|The value of Epsilon.|


### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Clamp(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>, min: <a data-footnote-ref href="#user-content-fn-127">Object</a>, max: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Clamp a value between a minimum and maximum value.
> 
> **Parameters**:
> - `value`: The value to clamp. Can be int or float.
> - `min`: The minimum value. Can be int or float.
> - `max`: The maximum value. Can be int or float.
> 
> **Returns**: The clamped value. Will be the same type as the inputs.
<pre class="language-typescript"><code class="lang-typescript">function Max(a: <a data-footnote-ref href="#user-content-fn-127">Object</a>, b: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Get the maximum of two values.
> 
> **Parameters**:
> - `a`: The first value. Can be int or float.
> - `b`: The second value. Can be int or float.
> 
> **Returns**: The maximum of the two values. Will be the same type as the inputs.
<pre class="language-typescript"><code class="lang-typescript">function Min(a: <a data-footnote-ref href="#user-content-fn-127">Object</a>, b: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Get the minimum of two values.
> 
> **Parameters**:
> - `a`: The first value. Can be int or float.
> - `b`: The second value. Can be int or float.
> 
> **Returns**: The minimum of the two values. Will be the same type as the inputs.
<pre class="language-typescript"><code class="lang-typescript">function Pow(a: float, b: float) -> float</code></pre>
> Raise a value to the power of another value.
> 
> **Parameters**:
> - `a`: The base value.
> - `b`: The exponent value.
> 
> **Returns**: The result of raising a to the power of b.
<pre class="language-typescript"><code class="lang-typescript">function Abs(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Get the absolute value of a number.
> 
> **Parameters**:
> - `value`: The number. Can be int or float.
> 
> **Returns**: The absolute value. Will be the same type as the input.
<pre class="language-typescript"><code class="lang-typescript">function Sqrt(value: float) -> float</code></pre>
> Get the square root of a number.
> 
> **Parameters**:
> - `value`: The value to get the square root of.
> 
> **Returns**: The square root of the value.
<pre class="language-typescript"><code class="lang-typescript">function Repeat(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>, max: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Modulo for floats.
> 
> **Parameters**:
> - `value`: The value to repeat.
> - `max`: The maximum value to repeat to.
> 
> **Returns**: The repeated value.
<pre class="language-typescript"><code class="lang-typescript">function Mod(a: int, b: int) -> int</code></pre>
> Get the remainder of a division operation.
> 
> **Parameters**:
> - `a`: The dividend.
> - `b`: The divisor.
> 
> **Returns**: The remainder of the division.
<pre class="language-typescript"><code class="lang-typescript">function Sin(angle: float) -> float</code></pre>
> Get the sine of an angle.
> 
> **Parameters**:
> - `angle`: The angle in degrees.
> 
> **Returns**: Value between -1 and 1.
<pre class="language-typescript"><code class="lang-typescript">function Cos(angle: float) -> float</code></pre>
> Get the cosine of an angle.
> 
> **Parameters**:
> - `angle`: The angle in degrees.
> 
> **Returns**: Value between -1 and 1.
<pre class="language-typescript"><code class="lang-typescript">function Tan(angle: float) -> float</code></pre>
> Get the tangent of an angle in radians.
> 
> **Parameters**:
> - `angle`: The angle in degrees.
> 
> **Returns**: The tangent of the angle.
<pre class="language-typescript"><code class="lang-typescript">function Asin(value: float) -> float</code></pre>
> Get the arcsine of a value in degrees.
> 
> **Parameters**:
> - `value`: The value (must be between -1 and 1).
> 
> **Returns**: The arcsine in degrees.
<pre class="language-typescript"><code class="lang-typescript">function Acos(value: float) -> float</code></pre>
> Get the arccosine of a value in degrees.
> 
> **Parameters**:
> - `value`: The value (must be between -1 and 1).
> 
> **Returns**: The arccosine in degrees.
<pre class="language-typescript"><code class="lang-typescript">function Atan(value: float) -> float</code></pre>
> Get the arctangent of a value in degrees.
> 
> **Parameters**:
> - `value`: The value to get the arctangent of.
> 
> **Returns**: The arctangent in degrees.
<pre class="language-typescript"><code class="lang-typescript">function Atan2(a: float, b: float) -> float</code></pre>
> Get the arctangent of a value in degrees.
> 
> **Parameters**:
> - `a`: The Y component.
> - `b`: The X component.
> 
> **Returns**: The arctangent in degrees.
<pre class="language-typescript"><code class="lang-typescript">function Ceil(value: float) -> int</code></pre>
> Get the smallest integer greater than or equal to a value.
> 
> **Parameters**:
> - `value`: The value to round up.
> 
> **Returns**: The smallest integer greater than or equal to the value.
<pre class="language-typescript"><code class="lang-typescript">function Floor(value: float) -> int</code></pre>
> Get the largest integer less than or equal to a value.
> 
> **Parameters**:
> - `value`: The value to round down.
> 
> **Returns**: The largest integer less than or equal to the value.
<pre class="language-typescript"><code class="lang-typescript">function Round(value: float) -> int</code></pre>
> Round a value to the nearest integer.
> 
> **Parameters**:
> - `value`: The value to round.
> 
> **Returns**: The rounded integer value.
<pre class="language-typescript"><code class="lang-typescript">function Deg2Rad(angle: float) -> float</code></pre>
> Convert an angle from degrees to radians.
> 
> **Parameters**:
> - `angle`: The angle in degrees.
> 
> **Returns**: The angle in radians.
<pre class="language-typescript"><code class="lang-typescript">function Rad2Deg(angle: float) -> float</code></pre>
> Convert an angle from radians to degrees.
> 
> **Parameters**:
> - `angle`: The angle in radians.
> 
> **Returns**: The angle in degrees.
<pre class="language-typescript"><code class="lang-typescript">function Lerp(a: float, b: float, t: float) -> float</code></pre>
> Linearly interpolate between two values.
> 
> **Parameters**:
> - `a`: The start value.
> - `b`: The end value.
> - `t`: The interpolation factor (clamped between 0 and 1).
> 
> **Returns**: The interpolated value.
<pre class="language-typescript"><code class="lang-typescript">function LerpUnclamped(a: float, b: float, t: float) -> float</code></pre>
> Linearly interpolate between two values without clamping.
> 
> **Parameters**:
> - `a`: The start value.
> - `b`: The end value.
> - `t`: The interpolation factor (not clamped).
> 
> **Returns**: The interpolated value.
<pre class="language-typescript"><code class="lang-typescript">function Sign(value: float) -> float</code></pre>
> Get the sign of a value.
> 
> **Parameters**:
> - `value`: The value to get the sign of.
> 
> **Returns**: The sign of the value (-1, 0, or 1).
<pre class="language-typescript"><code class="lang-typescript">function InverseLerp(a: float, b: float, value: float) -> float</code></pre>
> Get the inverse lerp of two values.
> 
> **Parameters**:
> - `a`: The start value.
> - `b`: The end value.
> - `value`: The value to find the interpolation factor for.
> 
> **Returns**: The interpolation factor.
<pre class="language-typescript"><code class="lang-typescript">function LerpAngle(a: float, b: float, t: float) -> float</code></pre>
> Linearly interpolate between two angles.
> 
> **Parameters**:
> - `a`: The start angle in degrees.
> - `b`: The end angle in degrees.
> - `t`: The interpolation factor (clamped between 0 and 1).
> 
> **Returns**: The interpolated angle.
<pre class="language-typescript"><code class="lang-typescript">function Log(value: float) -> float</code></pre>
> Get the natural logarithm of a value.
> 
> **Parameters**:
> - `value`: The value to get the logarithm of.
> 
> **Returns**: The natural logarithm of the value.
<pre class="language-typescript"><code class="lang-typescript">function MoveTowards(current: float, target: float, maxDelta: float) -> float</code></pre>
> Move a value towards a target value.
> 
> **Parameters**:
> - `current`: The current value.
> - `target`: The target value.
> - `maxDelta`: The maximum change allowed.
> 
> **Returns**: The new value moved towards the target.
<pre class="language-typescript"><code class="lang-typescript">function MoveTowardsAngle(current: float, target: float, maxDelta: float) -> float</code></pre>
> Move an angle towards a target angle.
> 
> **Parameters**:
> - `current`: The current angle in degrees.
> - `target`: The target angle in degrees.
> - `maxDelta`: The maximum change in degrees allowed.
> 
> **Returns**: The new angle moved towards the target.
<pre class="language-typescript"><code class="lang-typescript">function PingPong(t: float, length: float) -> float</code></pre>
> Get the ping pong value of a time value.
> 
> **Parameters**:
> - `t`: The time value.
> - `length`: The length of the ping pong cycle.
> 
> **Returns**: The ping pong value.
<pre class="language-typescript"><code class="lang-typescript">function Exp(value: float) -> float</code></pre>
> Get the exponential value of a number.
> 
> **Parameters**:
> - `value`: The value to exponentiate.
> 
> **Returns**: The exponential value.
<pre class="language-typescript"><code class="lang-typescript">function SmoothStep(a: float, b: float, t: float) -> float</code></pre>
> Smoothly step between two values.
> 
> **Parameters**:
> - `a`: The start value.
> - `b`: The end value.
> - `t`: The interpolation factor (clamped between 0 and 1).
> 
> **Returns**: The smoothly interpolated value.
<pre class="language-typescript"><code class="lang-typescript">function BitwiseAnd(a: int, b: int) -> int</code></pre>
> Perform a bitwise AND operation.
> 
> **Parameters**:
> - `a`: The first integer.
> - `b`: The second integer.
> 
> **Returns**: The result of the bitwise AND operation.
<pre class="language-typescript"><code class="lang-typescript">function BitwiseOr(a: int, b: int) -> int</code></pre>
> Perform a bitwise OR operation.
> 
> **Parameters**:
> - `a`: The first integer.
> - `b`: The second integer.
> 
> **Returns**: The result of the bitwise OR operation.
<pre class="language-typescript"><code class="lang-typescript">function BitwiseXor(a: int, b: int) -> int</code></pre>
> Perform a bitwise XOR operation.
> 
> **Parameters**:
> - `a`: The first integer.
> - `b`: The second integer.
> 
> **Returns**: The result of the bitwise XOR operation.
<pre class="language-typescript"><code class="lang-typescript">function BitwiseNot(value: int) -> int</code></pre>
> Perform a bitwise NOT operation.
> 
> **Parameters**:
> - `value`: The integer to negate.
> 
> **Returns**: The result of the bitwise NOT operation.
<pre class="language-typescript"><code class="lang-typescript">function BitwiseLeftShift(value: int, shift: int) -> int</code></pre>
> Shift bits to the left.
> 
> **Parameters**:
> - `value`: The integer to shift.
> - `shift`: The number of bits to shift left.
> 
> **Returns**: The result of the left shift operation.
<pre class="language-typescript"><code class="lang-typescript">function BitwiseRightShift(value: int, shift: int) -> int</code></pre>
> Shift bits to the right.
> 
> **Parameters**:
> - `value`: The integer to shift.
> - `shift`: The number of bits to shift right.
> 
> **Returns**: The result of the right shift operation.

[^0]: [Color](../Collections/Color.md)
[^1]: [Dict](../Collections/Dict.md)
[^2]: [LineCastHitResult](../Collections/LineCastHitResult.md)
[^3]: [List](../Collections/List.md)
[^4]: [Quaternion](../Collections/Quaternion.md)
[^5]: [Range](../Collections/Range.md)
[^6]: [Set](../Collections/Set.md)
[^7]: [Vector2](../Collections/Vector2.md)
[^8]: [Vector3](../Collections/Vector3.md)
[^9]: [Animation](../Component/Animation.md)
[^10]: [Animator](../Component/Animator.md)
[^11]: [AudioSource](../Component/AudioSource.md)
[^12]: [Collider](../Component/Collider.md)
[^13]: [Collision](../Component/Collision.md)
[^14]: [LightBuiltin](../Component/LightBuiltin.md)
[^15]: [LineRenderer](../Component/LineRenderer.md)
[^16]: [LodBuiltin](../Component/LodBuiltin.md)
[^17]: [MapTargetable](../Component/MapTargetable.md)
[^18]: [NavmeshObstacleBuiltin](../Component/NavmeshObstacleBuiltin.md)
[^19]: [PhysicsMaterialBuiltin](../Component/PhysicsMaterialBuiltin.md)
[^20]: [RigidbodyBuiltin](../Component/RigidbodyBuiltin.md)
[^21]: [VideoPlayer](../Component/VideoPlayer.md)
[^22]: [Character](../Entities/Character.md)
[^23]: [Horse](../Entities/Horse.md)
[^24]: [Human](../Entities/Human.md)
[^25]: [MapObject](../Entities/MapObject.md)
[^26]: [NetworkView](../Entities/NetworkView.md)
[^27]: [Player](../Entities/Player.md)
[^28]: [Prefab](../Entities/Prefab.md)
[^29]: [Shifter](../Entities/Shifter.md)
[^30]: [Titan](../Entities/Titan.md)
[^31]: [Transform](../Entities/Transform.md)
[^32]: [WallColossal](../Entities/WallColossal.md)
[^33]: [AlignEnum](../Enums/AlignEnum.md)
[^34]: [AngleUnitEnum](../Enums/AngleUnitEnum.md)
[^35]: [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md)
[^36]: [AspectRatioEnum](../Enums/AspectRatioEnum.md)
[^37]: [CameraModeEnum](../Enums/CameraModeEnum.md)
[^38]: [CharacterTypeEnum](../Enums/CharacterTypeEnum.md)
[^39]: [CollideModeEnum](../Enums/CollideModeEnum.md)
[^40]: [CollideWithEnum](../Enums/CollideWithEnum.md)
[^41]: [CollisionDetectionModeEnum](../Enums/CollisionDetectionModeEnum.md)
[^42]: [DummyAnimationEnum](../Enums/DummyAnimationEnum.md)
[^43]: [EffectNameEnum](../Enums/EffectNameEnum.md)
[^44]: [ErenAnimationEnum](../Enums/ErenAnimationEnum.md)
[^45]: [FlexDirectionEnum](../Enums/FlexDirectionEnum.md)
[^46]: [FontScaleModeEnum](../Enums/FontScaleModeEnum.md)
[^47]: [FontStyleEnum](../Enums/FontStyleEnum.md)
[^48]: [ForceModeEnum](../Enums/ForceModeEnum.md)
[^49]: [GradientModeEnum](../Enums/GradientModeEnum.md)
[^50]: [HandStateEnum](../Enums/HandStateEnum.md)
[^51]: [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
[^52]: [HumanAnimationEnum](../Enums/HumanAnimationEnum.md)
[^53]: [HumanParticleEffectEnum](../Enums/HumanParticleEffectEnum.md)
[^54]: [HumanSoundEnum](../Enums/HumanSoundEnum.md)
[^55]: [HumanStateEnum](../Enums/HumanStateEnum.md)
[^56]: [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md)
[^57]: [InputCategoryEnum](../Enums/InputCategoryEnum.md)
[^58]: [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
[^59]: [InputGeneralEnum](../Enums/InputGeneralEnum.md)
[^60]: [InputHumanEnum](../Enums/InputHumanEnum.md)
[^61]: [InputInteractionEnum](../Enums/InputInteractionEnum.md)
[^62]: [InputTitanEnum](../Enums/InputTitanEnum.md)
[^63]: [JustifyEnum](../Enums/JustifyEnum.md)
[^64]: [LanguageEnum](../Enums/LanguageEnum.md)
[^65]: [LineAlignmentEnum](../Enums/LineAlignmentEnum.md)
[^66]: [LineTextureModeEnum](../Enums/LineTextureModeEnum.md)
[^67]: [LoadoutEnum](../Enums/LoadoutEnum.md)
[^68]: [OutlineModeEnum](../Enums/OutlineModeEnum.md)
[^69]: [OverflowEnum](../Enums/OverflowEnum.md)
[^70]: [PhysicMaterialCombineEnum](../Enums/PhysicMaterialCombineEnum.md)
[^71]: [PlayerStatusEnum](../Enums/PlayerStatusEnum.md)
[^72]: [ProfileIconEnum](../Enums/ProfileIconEnum.md)
[^73]: [ProjectileNameEnum](../Enums/ProjectileNameEnum.md)
[^74]: [ScaleModeEnum](../Enums/ScaleModeEnum.md)
[^75]: [ScrollElasticityEnum](../Enums/ScrollElasticityEnum.md)
[^76]: [ShadowCastingModeEnum](../Enums/ShadowCastingModeEnum.md)
[^77]: [ShifterSoundEnum](../Enums/ShifterSoundEnum.md)
[^78]: [ShifterTypeEnum](../Enums/ShifterTypeEnum.md)
[^79]: [SliderDirectionEnum](../Enums/SliderDirectionEnum.md)
[^80]: [SpecialEnum](../Enums/SpecialEnum.md)
[^81]: [SteamStateEnum](../Enums/SteamStateEnum.md)
[^82]: [StunStateEnum](../Enums/StunStateEnum.md)
[^83]: [TSKillSoundEnum](../Enums/TSKillSoundEnum.md)
[^84]: [TeamEnum](../Enums/TeamEnum.md)
[^85]: [TextAlignEnum](../Enums/TextAlignEnum.md)
[^86]: [TextOverflowEnum](../Enums/TextOverflowEnum.md)
[^87]: [TitanAnimationEnum](../Enums/TitanAnimationEnum.md)
[^88]: [TitanDeathTypeEnum](../Enums/TitanDeathTypeEnum.md)
[^89]: [TitanSoundEnum](../Enums/TitanSoundEnum.md)
[^90]: [TitanTypeEnum](../Enums/TitanTypeEnum.md)
[^91]: [UILabelEnum](../Enums/UILabelEnum.md)
[^92]: [UnityComponentEnum](../Enums/UnityComponentEnum.md)
[^93]: [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md)
[^94]: [WeaponEnum](../Enums/WeaponEnum.md)
[^95]: [WrapEnum](../Enums/WrapEnum.md)
[^96]: [Camera](../Game/Camera.md)
[^97]: [Commands](../Game/Commands.md)
[^98]: [Cutscene](../Game/Cutscene.md)
[^99]: [ExperienceScore](../Game/ExperienceScore.md)
[^100]: [Game](../Game/Game.md)
[^101]: [Input](../Game/Input.md)
[^102]: [Locale](../Game/Locale.md)
[^103]: [Map](../Game/Map.md)
[^104]: [Network](../Game/Network.md)
[^105]: [PersistentData](../Game/PersistentData.md)
[^106]: [Physics](../Game/Physics.md)
[^107]: [RoomData](../Game/RoomData.md)
[^108]: [Service](../Game/Service.md)
[^109]: [Time](../Game/Time.md)
[^110]: [Button](../UIElements/Button.md)
[^111]: [Dropdown](../UIElements/Dropdown.md)
[^112]: [Icon](../UIElements/Icon.md)
[^113]: [Image](../UIElements/Image.md)
[^114]: [Label](../UIElements/Label.md)
[^115]: [ProgressBar](../UIElements/ProgressBar.md)
[^116]: [ScrollView](../UIElements/ScrollView.md)
[^117]: [Slider](../UIElements/Slider.md)
[^118]: [TextField](../UIElements/TextField.md)
[^119]: [Toggle](../UIElements/Toggle.md)
[^120]: [UI](../UIElements/UI.md)
[^121]: [VisualElement](../UIElements/VisualElement.md)
[^122]: [Convert](../Utility/Convert.md)
[^123]: [Json](../Utility/Json.md)
[^124]: [Math](../Utility/Math.md)
[^125]: [Random](../Utility/Random.md)
[^126]: [String](../Utility/String.md)
[^127]: [Object](../objects/Object.md)
[^128]: [Component](../objects/Component.md)
