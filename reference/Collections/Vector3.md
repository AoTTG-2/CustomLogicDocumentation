# Vector3
Inherits from [Object](../objects/Object.md)

Represents a 3D vector with X, Y, and Z components. Supports mathematical operations and implements copy semantics.

### Remarks
Overloads operators: 
`__Copy__`, `+`, `-`, `*`, `/`, `==`, `__Hash__`
### Initialization
```csharp
Vector3() // Default constructor, Initializes the Vector3 to (0, 0, 0).
Vector3(xyz: float) // Initializes the Vector3 to (xyz, xyz, xyz).
Vector3(x: float, y: float) // Initializes the Vector3 to (x, y, 0).
Vector3(x: float, y: float, z: float) // Initializes the Vector3 to (x, y, z).
```

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|X|float|False|The X component of the vector.|
|Y|float|False|The Y component of the vector.|
|Z|float|False|The Z component of the vector.|
|Normalized|[Vector3](../Collections/Vector3.md)|True|Returns a normalized copy of this vector (magnitude of 1).|
|Magnitude|float|True|Returns the length of this vector.|
|SqrMagnitude|float|True|Returns the squared length of this vector (faster than Magnitude).|


### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Zero|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(0, 0, 0).|
|One|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(1, 1, 1).|
|Up|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(0, 1, 0).|
|Down|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(0, -1, 0).|
|Left|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(-1, 0, 0).|
|Right|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(1, 0, 0).|
|Forward|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(0, 0, 1).|
|Back|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(0, 0, -1).|
|NegativeInfinity|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(float.NegativeInfinity, float.NegativeInfinity, float.NegativeInfinity).|
|PositiveInfinity|[Vector3](../Collections/Vector3.md)|True|Shorthand for writing Vector3(float.PositiveInfinity, float.PositiveInfinity, float.PositiveInfinity).|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Set(x: float, y: float, z: float)</code></pre>
> Sets the X, Y, and Z components of the vector.
> 
> **Parameters**:
> - `x`: The X component.
> - `y`: The Y component.
> - `z`: The Z component.
> 
<pre class="language-typescript"><code class="lang-typescript">function Scale(scale: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>

{% hint style="warning" %}
**Obsolete**: Use multiply operator instead
{% endhint %}

> Scales the vector by a float or Vector3.
> 
> **Parameters**:
> - `scale`: The scale value (float or Vector3).
> 
> **Returns**: A new scaled vector.

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Angle(from: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, to: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> float</code></pre>
> Calculates the angle between two vectors.
> 
> **Parameters**:
> - `from`: The vector from which the angular difference is measured.
> - `to`: The vector to which the angular difference is measured.
> 
<pre class="language-typescript"><code class="lang-typescript">function ClampMagnitude(vector: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, maxLength: float) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Clamps the magnitude of a vector to a maximum value.
> 
> **Parameters**:
> - `vector`: The vector to clamp.
> - `maxLength`: The maximum length of the vector.
> 
<pre class="language-typescript"><code class="lang-typescript">function Cross(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Calculates the cross product of two vectors.
> 
> **Parameters**:
> - `a`: The first vector.
> - `b`: The second vector.
> 
<pre class="language-typescript"><code class="lang-typescript">function Distance(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> float</code></pre>
> Calculates the distance between two points.
> 
> **Parameters**:
> - `a`: The first point.
> - `b`: The second point.
> 
<pre class="language-typescript"><code class="lang-typescript">function Dot(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> float</code></pre>
> Calculates the dot product of two vectors.
> 
> **Parameters**:
> - `a`: The first vector.
> - `b`: The second vector.
> 
<pre class="language-typescript"><code class="lang-typescript">function Lerp(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Linearly interpolates between two vectors.
> 
> **Parameters**:
> - `a`: The start value.
> - `b`: The end value.
> - `t`: The interpolation factor (clamped between 0 and 1).
> 
<pre class="language-typescript"><code class="lang-typescript">function LerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Linearly interpolates between two vectors without clamping.
> 
> **Parameters**:
> - `a`: The start value.
> - `b`: The end value.
> - `t`: The interpolation factor (not clamped).
> 
<pre class="language-typescript"><code class="lang-typescript">function Max(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Returns a vector that is made from the largest components of two vectors.
> 
> **Parameters**:
> - `a`: The first vector.
> - `b`: The second vector.
> 
<pre class="language-typescript"><code class="lang-typescript">function Min(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Returns a vector that is made from the smallest components of two vectors.
> 
> **Parameters**:
> - `a`: The first vector.
> - `b`: The second vector.
> 
<pre class="language-typescript"><code class="lang-typescript">function MoveTowards(current: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, target: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, maxDistanceDelta: float) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Moves a point towards a target position.
> 
> **Parameters**:
> - `current`: The current position.
> - `target`: The target position.
> - `maxDistanceDelta`: The maximum distance to move.
> 
<pre class="language-typescript"><code class="lang-typescript">function Normalize(value: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Returns a normalized copy of the vector.
> 
> **Parameters**:
> - `value`: The vector to normalize.
> 
<pre class="language-typescript"><code class="lang-typescript">function OrthoNormalize(normal: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, tangent: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>)</code></pre>
> Orthonormalizes two vectors (normalizes the normal vector and makes the tangent vector orthogonal to it).
> 
> **Parameters**:
> - `normal`: The normal vector (will be normalized).
> - `tangent`: The tangent vector (will be normalized and made orthogonal to normal).
> 
<pre class="language-typescript"><code class="lang-typescript">function Project(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Projects a vector onto another vector.
> 
> **Parameters**:
> - `a`: The vector to project.
> - `b`: The vector to project onto.
> 
<pre class="language-typescript"><code class="lang-typescript">function ProjectOnPlane(vector: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, plane: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Projects a vector onto a plane defined by a normal vector.
> 
> **Parameters**:
> - `vector`: The vector to project.
> - `plane`: The plane normal vector.
> 
<pre class="language-typescript"><code class="lang-typescript">function Reflect(inDirection: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, inNormal: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Reflects a vector off a plane defined by a normal vector.
> 
> **Parameters**:
> - `inDirection`: The incoming direction vector.
> - `inNormal`: The normal vector of the surface.
> 
<pre class="language-typescript"><code class="lang-typescript">function RotateTowards(current: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, target: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, maxRadiansDelta: float, maxMagnitudeDelta: float) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Rotates a vector towards a target vector.
> 
> **Parameters**:
> - `current`: The current direction vector.
> - `target`: The target direction vector.
> - `maxRadiansDelta`: The maximum change in radians.
> - `maxMagnitudeDelta`: The maximum change in magnitude.
> 
<pre class="language-typescript"><code class="lang-typescript">function SignedAngle(from: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, to: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, axis: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> float</code></pre>
> Calculates the signed angle between two vectors.
> 
> **Parameters**:
> - `from`: The vector from which the angular difference is measured.
> - `to`: The vector to which the angular difference is measured.
> - `axis`: The axis around which the rotation is measured.
> 
<pre class="language-typescript"><code class="lang-typescript">function Slerp(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Spherically interpolates between two vectors.
> 
> **Parameters**:
> - `a`: The start value.
> - `b`: The end value.
> - `t`: The interpolation factor (clamped between 0 and 1).
> 
<pre class="language-typescript"><code class="lang-typescript">function SlerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Spherically interpolates between two vectors without clamping.
> 
> **Parameters**:
> - `a`: The start value.
> - `b`: The end value.
> - `t`: The interpolation factor (not clamped).
> 
<pre class="language-typescript"><code class="lang-typescript">function SmoothDamp(current: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, target: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, currentVelocity: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, smoothTime: float, maxSpeed: float) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Smoothly dampens a vector towards a target over time.
> 
> **Parameters**:
> - `current`: The current position.
> - `target`: The target position.
> - `currentVelocity`: The current velocity (modified by the function).
> - `smoothTime`: The time it takes to reach the target (approximately).
> - `maxSpeed`: The maximum speed.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetRotationDirection(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Gets the direction vector transformed by a rotation.
> 
> **Parameters**:
> - `a`: The reference rotation vector (e.g., forward direction).
> - `b`: The vector to transform relative to the reference.
> 
> **Returns**: A new direction vector.
<pre class="language-typescript"><code class="lang-typescript">function Multiply(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>

{% hint style="warning" %}
**Obsolete**: Use multiply operator instead
{% endhint %}

> Multiplies two vectors component-wise.
> 
> **Parameters**:
> - `a`: The first vector.
> - `b`: The second vector.
> 
> **Returns**: A new vector with multiplied components.
<pre class="language-typescript"><code class="lang-typescript">function Divide(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>

{% hint style="warning" %}
**Obsolete**: Use divide operator instead
{% endhint %}

> Divides two vectors component-wise.
> 
> **Parameters**:
> - `a`: The first vector.
> - `b`: The second vector.
> 
> **Returns**: A new vector with divided components.

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
[^23]: [Human](../Entities/Human.md)
[^24]: [MapObject](../Entities/MapObject.md)
[^25]: [NetworkView](../Entities/NetworkView.md)
[^26]: [Player](../Entities/Player.md)
[^27]: [Prefab](../Entities/Prefab.md)
[^28]: [Shifter](../Entities/Shifter.md)
[^29]: [Titan](../Entities/Titan.md)
[^30]: [Transform](../Entities/Transform.md)
[^31]: [WallColossal](../Entities/WallColossal.md)
[^32]: [AlignEnum](../Enums/AlignEnum.md)
[^33]: [AngleUnitEnum](../Enums/AngleUnitEnum.md)
[^34]: [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md)
[^35]: [AspectRatioEnum](../Enums/AspectRatioEnum.md)
[^36]: [CameraModeEnum](../Enums/CameraModeEnum.md)
[^37]: [CharacterTypeEnum](../Enums/CharacterTypeEnum.md)
[^38]: [CollideModeEnum](../Enums/CollideModeEnum.md)
[^39]: [CollideWithEnum](../Enums/CollideWithEnum.md)
[^40]: [CollisionDetectionModeEnum](../Enums/CollisionDetectionModeEnum.md)
[^41]: [DummyAnimationEnum](../Enums/DummyAnimationEnum.md)
[^42]: [EffectNameEnum](../Enums/EffectNameEnum.md)
[^43]: [ErenAnimationEnum](../Enums/ErenAnimationEnum.md)
[^44]: [FlexDirectionEnum](../Enums/FlexDirectionEnum.md)
[^45]: [FontScaleModeEnum](../Enums/FontScaleModeEnum.md)
[^46]: [FontStyleEnum](../Enums/FontStyleEnum.md)
[^47]: [ForceModeEnum](../Enums/ForceModeEnum.md)
[^48]: [GradientModeEnum](../Enums/GradientModeEnum.md)
[^49]: [HandStateEnum](../Enums/HandStateEnum.md)
[^50]: [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
[^51]: [HumanAnimationEnum](../Enums/HumanAnimationEnum.md)
[^52]: [HumanParticleEffectEnum](../Enums/HumanParticleEffectEnum.md)
[^53]: [HumanSoundEnum](../Enums/HumanSoundEnum.md)
[^54]: [HumanStateEnum](../Enums/HumanStateEnum.md)
[^55]: [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md)
[^56]: [InputCategoryEnum](../Enums/InputCategoryEnum.md)
[^57]: [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
[^58]: [InputGeneralEnum](../Enums/InputGeneralEnum.md)
[^59]: [InputHumanEnum](../Enums/InputHumanEnum.md)
[^60]: [InputInteractionEnum](../Enums/InputInteractionEnum.md)
[^61]: [InputTitanEnum](../Enums/InputTitanEnum.md)
[^62]: [JustifyEnum](../Enums/JustifyEnum.md)
[^63]: [LanguageEnum](../Enums/LanguageEnum.md)
[^64]: [LineAlignmentEnum](../Enums/LineAlignmentEnum.md)
[^65]: [LineTextureModeEnum](../Enums/LineTextureModeEnum.md)
[^66]: [LoadoutEnum](../Enums/LoadoutEnum.md)
[^67]: [OutlineModeEnum](../Enums/OutlineModeEnum.md)
[^68]: [OverflowEnum](../Enums/OverflowEnum.md)
[^69]: [PhysicMaterialCombineEnum](../Enums/PhysicMaterialCombineEnum.md)
[^70]: [PlayerStatusEnum](../Enums/PlayerStatusEnum.md)
[^71]: [ProfileIconEnum](../Enums/ProfileIconEnum.md)
[^72]: [ProjectileNameEnum](../Enums/ProjectileNameEnum.md)
[^73]: [ScaleModeEnum](../Enums/ScaleModeEnum.md)
[^74]: [ScrollElasticityEnum](../Enums/ScrollElasticityEnum.md)
[^75]: [ShadowCastingModeEnum](../Enums/ShadowCastingModeEnum.md)
[^76]: [ShifterSoundEnum](../Enums/ShifterSoundEnum.md)
[^77]: [ShifterTypeEnum](../Enums/ShifterTypeEnum.md)
[^78]: [SliderDirectionEnum](../Enums/SliderDirectionEnum.md)
[^79]: [SpecialEnum](../Enums/SpecialEnum.md)
[^80]: [SteamStateEnum](../Enums/SteamStateEnum.md)
[^81]: [StunStateEnum](../Enums/StunStateEnum.md)
[^82]: [TeamEnum](../Enums/TeamEnum.md)
[^83]: [TextAlignEnum](../Enums/TextAlignEnum.md)
[^84]: [TextOverflowEnum](../Enums/TextOverflowEnum.md)
[^85]: [TitanAnimationEnum](../Enums/TitanAnimationEnum.md)
[^86]: [TitanSoundEnum](../Enums/TitanSoundEnum.md)
[^87]: [TitanTypeEnum](../Enums/TitanTypeEnum.md)
[^88]: [TSKillSoundEnum](../Enums/TSKillSoundEnum.md)
[^89]: [UILabelEnum](../Enums/UILabelEnum.md)
[^90]: [UnityComponentEnum](../Enums/UnityComponentEnum.md)
[^91]: [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md)
[^92]: [WeaponEnum](../Enums/WeaponEnum.md)
[^93]: [WrapEnum](../Enums/WrapEnum.md)
[^94]: [Camera](../Game/Camera.md)
[^95]: [Cutscene](../Game/Cutscene.md)
[^96]: [Game](../Game/Game.md)
[^97]: [Input](../Game/Input.md)
[^98]: [Locale](../Game/Locale.md)
[^99]: [Map](../Game/Map.md)
[^100]: [Network](../Game/Network.md)
[^101]: [PersistentData](../Game/PersistentData.md)
[^102]: [Physics](../Game/Physics.md)
[^103]: [RoomData](../Game/RoomData.md)
[^104]: [Time](../Game/Time.md)
[^105]: [Button](../UIElements/Button.md)
[^106]: [Dropdown](../UIElements/Dropdown.md)
[^107]: [Icon](../UIElements/Icon.md)
[^108]: [Image](../UIElements/Image.md)
[^109]: [Label](../UIElements/Label.md)
[^110]: [ProgressBar](../UIElements/ProgressBar.md)
[^111]: [ScrollView](../UIElements/ScrollView.md)
[^112]: [Slider](../UIElements/Slider.md)
[^113]: [TextField](../UIElements/TextField.md)
[^114]: [Toggle](../UIElements/Toggle.md)
[^115]: [UI](../UIElements/UI.md)
[^116]: [VisualElement](../UIElements/VisualElement.md)
[^117]: [Convert](../Utility/Convert.md)
[^118]: [Json](../Utility/Json.md)
[^119]: [Math](../Utility/Math.md)
[^120]: [Random](../Utility/Random.md)
[^121]: [String](../Utility/String.md)
[^122]: [Object](../objects/Object.md)
[^123]: [Component](../objects/Component.md)
