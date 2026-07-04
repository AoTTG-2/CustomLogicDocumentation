# Transform
Inherits from [Object](../objects/Object.md)

Represents a transform.

### Remarks
Overloads operators: 
`==`, `__Hash__`
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Position|[Vector3](../Collections/Vector3.md)|False|Gets or sets the position of the transform.|
|LocalPosition|[Vector3](../Collections/Vector3.md)|False|Gets or sets the local position of the transform.|
|Rotation|[Vector3](../Collections/Vector3.md)|False|Gets or sets the rotation of the transform.|
|LocalRotation|[Vector3](../Collections/Vector3.md)|False|Gets or sets the local rotation of the transform.|
|QuaternionRotation|[Quaternion](../Collections/Quaternion.md)|False|Gets or sets the quaternion rotation of the transform.|
|QuaternionLocalRotation|[Quaternion](../Collections/Quaternion.md)|False|Gets or sets the quaternion local rotation of the transform.|
|Scale|[Vector3](../Collections/Vector3.md)|False|Gets or sets the scale of the transform.|
|Forward|[Vector3](../Collections/Vector3.md)|False|Gets the forward vector of the transform.|
|Up|[Vector3](../Collections/Vector3.md)|False|Gets the up vector of the transform.|
|Right|[Vector3](../Collections/Vector3.md)|False|Gets the right vector of the transform.|
|Parent|[Transform](../Entities/Transform.md)|False|Sets the parent of the transform.|
|Name|string|True|Gets the name of the transform.|
|Layer|int|False|Gets the Physics Layer of the transform.|
|Animation|[Animation](../Component/Animation.md)|True|The Animation attached to this transform, returns null if there is none.|
|Animator|[Animator](../Component/Animator.md)|True|The Animator attached to this transform, returns null if there is none.|
|AudioSource|[AudioSource](../Component/AudioSource.md)|True|The AudioSource attached to this transform, returns null if there is none.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function GetTransform(name: string) -> <a data-footnote-ref href="#user-content-fn-30">Transform</a></code></pre>
> Gets the transform of the specified child.
> 
> **Parameters**:
> - `name`: The name of the child transform to find.
> 
> **Returns**: The child transform if found, null otherwise.
<pre class="language-typescript"><code class="lang-typescript">function GetTransforms() -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-30">Transform</a>></code></pre>
> Gets all child transforms.
> 
> **Returns**: A list of all child transforms.
<pre class="language-typescript"><code class="lang-typescript">function IsPlayingAnimation(anim: string) -> bool</code></pre>
> Checks if the given animation is playing.
> 
> **Parameters**:
> - `anim`: The name of the animation to check. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> 
> **Returns**: True if the animation is playing, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function PlayAnimation(anim: string, fade: float = 0.1)</code></pre>
> Plays the specified animation.
> 
> **Parameters**:
> - `anim`: The name of the animation to play. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> - `fade`: The fade time in seconds for cross-fading (default: 0.1).
> 
<pre class="language-typescript"><code class="lang-typescript">function GetAnimationLength(anim: string) -> float</code></pre>
> Gets the length of the specified animation.
> 
> **Parameters**:
> - `anim`: The name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> 
> **Returns**: The length of the animation in seconds, or -1 if not found.
<pre class="language-typescript"><code class="lang-typescript">function PlaySound()</code></pre>
> Plays the sound.
> 
<pre class="language-typescript"><code class="lang-typescript">function StopSound()</code></pre>
> Stops the sound.
> 
<pre class="language-typescript"><code class="lang-typescript">function ToggleParticle(enabled: bool)</code></pre>
> Toggles the particle system.
> 
> **Parameters**:
> - `enabled`: Whether to enable or disable the particle emission.
> 
<pre class="language-typescript"><code class="lang-typescript">function InverseTransformDirection(direction: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Transforms a direction from world space to local space.
> 
> **Parameters**:
> - `direction`: The direction vector in world space.
> 
> **Returns**: The direction in local space.
<pre class="language-typescript"><code class="lang-typescript">function InverseTransformPoint(point: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Transforms a position from world space to local space.
> 
> **Parameters**:
> - `point`: The point in world space.
> 
> **Returns**: The position in local space.
<pre class="language-typescript"><code class="lang-typescript">function TransformDirection(direction: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Transforms a direction from local space to world space.
> 
> **Parameters**:
> - `direction`: The direction vector in local space.
> 
> **Returns**: The direction in world space.
<pre class="language-typescript"><code class="lang-typescript">function TransformPoint(point: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Transforms a position from local space to world space.
> 
> **Parameters**:
> - `point`: The point in local space.
> 
> **Returns**: The position in world space.
<pre class="language-typescript"><code class="lang-typescript">function Rotate(rotation: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>)</code></pre>
> Rotates the transform by the given rotation in euler angles.
> 
> **Parameters**:
> - `rotation`: The rotation in euler angles to apply.
> 
<pre class="language-typescript"><code class="lang-typescript">function RotateAround(point: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, axis: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, angle: float)</code></pre>
> Rotates the transform around a point by the given angle.
> 
> **Parameters**:
> - `point`: The point to rotate around.
> - `axis`: The axis to rotate around.
> - `angle`: The angle in degrees to rotate.
> 
<pre class="language-typescript"><code class="lang-typescript">function LookAt(target: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>)</code></pre>
> Rotates the transform to look at the target position.
> 
> **Parameters**:
> - `target`: The world position to look at.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetRenderersEnabled(enabled: bool)</code></pre>
> Sets the enabled state of all child renderers.
> 
> **Parameters**:
> - `enabled`: Whether to enable or disable the renderers.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetColliders(recursive: bool = False) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-12">Collider</a>></code></pre>
> Gets colliders of the transform.
> 
> **Parameters**:
> - `recursive`: If true, includes colliders from all children recursively (default: false).
> 
> **Returns**: A list of colliders.
<pre class="language-typescript"><code class="lang-typescript">function SetActive(active: bool)</code></pre>

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
