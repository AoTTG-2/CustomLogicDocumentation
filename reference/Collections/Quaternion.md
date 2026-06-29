# Quaternion
Inherits from [Object](../objects/Object.md)

Represents a quaternion.

### Remarks
Overloads operators: 
`__Copy__`, `*`, `==`, `__Hash__`
### Initialization
```csharp
Quaternion() // Default constructor, creates an identity quaternion (no rotation).
Quaternion(x: float, y: float, z: float, w: float) // Creates a new Quaternion from the given values.
```

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|X|float|False|The X component of the quaternion.|
|Y|float|False|The Y component of the quaternion.|
|Z|float|False|The Z component of the quaternion.|
|W|float|False|The W component of the quaternion.|
|Euler|[Vector3](../Collections/Vector3.md)|False|Returns or sets the euler angle representation of the rotation.|


### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Identity|[Quaternion](../Collections/Quaternion.md)|True|The identity rotation (no rotation).|


### Methods

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Lerp(a: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, b: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Linearly interpolates between two rotations.
> 
> **Parameters**:
> - `a`: The start rotation.
> - `b`: The end rotation.
> - `t`: The interpolation factor (clamped between 0 and 1).
> 
<pre class="language-typescript"><code class="lang-typescript">function LerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, b: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Linearly interpolates between two rotations without clamping.
> 
> **Parameters**:
> - `a`: The start rotation.
> - `b`: The end rotation.
> - `t`: The interpolation factor (not clamped).
> 
> **Returns**: The interpolated quaternion.
<pre class="language-typescript"><code class="lang-typescript">function Slerp(a: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, b: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Spherically interpolates between two rotations.
> 
> **Parameters**:
> - `a`: The start rotation.
> - `b`: The end rotation.
> - `t`: The interpolation factor (clamped between 0 and 1).
> 
> **Returns**: The interpolated quaternion.
<pre class="language-typescript"><code class="lang-typescript">function SlerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, b: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Spherically interpolates between two rotations without clamping.
> 
> **Parameters**:
> - `a`: The start rotation.
> - `b`: The end rotation.
> - `t`: The interpolation factor (not clamped).
> 
> **Returns**: The interpolated quaternion.
<pre class="language-typescript"><code class="lang-typescript">function FromEuler(euler: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Creates a rotation from euler angles.
> 
> **Parameters**:
> - `euler`: The euler angles in degrees (x, y, z).
> 
> **Returns**: A quaternion representing the rotation.
<pre class="language-typescript"><code class="lang-typescript">function LookRotation(forward: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, upwards: <a data-footnote-ref href="#user-content-fn-8">Vector3</a> = null) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Creates a rotation that looks in the specified direction.
> 
> **Parameters**:
> - `forward`: The forward direction vector.
> - `upwards`: Optional. The upwards direction vector (default: Vector3.up).
> 
> **Returns**: A quaternion representing the rotation.
<pre class="language-typescript"><code class="lang-typescript">function FromToRotation(a: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Creates a rotation from one direction to another.
> 
> **Parameters**:
> - `a`: The source direction vector.
> - `b`: The target direction vector.
> 
> **Returns**: A quaternion representing the rotation.
<pre class="language-typescript"><code class="lang-typescript">function Inverse(q: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Returns the inverse of a quaternion.
> 
> **Parameters**:
> - `q`: The quaternion to invert.
> 
> **Returns**: The inverse quaternion.
<pre class="language-typescript"><code class="lang-typescript">function RotateTowards(from: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, to: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, maxDegreesDelta: float) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Rotates a rotation towards a target rotation.
> 
> **Parameters**:
> - `from`: The current rotation.
> - `to`: The target rotation.
> - `maxDegreesDelta`: The maximum change in degrees.
> 
> **Returns**: The rotated quaternion.
<pre class="language-typescript"><code class="lang-typescript">function AngleAxis(angle: float, axis: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-4">Quaternion</a></code></pre>
> Creates a rotation that rotates around a specified axis by a specified angle.
> 
> **Parameters**:
> - `angle`: The angle in degrees.
> - `axis`: The axis to rotate around.
> 
> **Returns**: A quaternion representing the rotation.
<pre class="language-typescript"><code class="lang-typescript">function Angle(a: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, b: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>) -> float</code></pre>
> Calculates the angle between two rotations.
> 
> **Parameters**:
> - `a`: The first rotation.
> - `b`: The second rotation.
> 
> **Returns**: The angle in degrees.

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
