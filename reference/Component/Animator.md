# Animator

Represents an Animator component for controlling animations using Animator Controller.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|DeltaPosition|[Vector3](../Collections/Vector3.md)|True|Returns the delta position of the avatar.|
|DeltaRotation|[Quaternion](../Collections/Quaternion.md)|True|Returns the delta rotation of the avatar.|
|HasRootMotion|bool|True|Animator has root motion.|
|ApplyRootMotion|bool|False|Whether root motion should be applied.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function ApplyBuiltinRootMotion()</code></pre>
> Apply the default Root Motion.
> 
<pre class="language-typescript"><code class="lang-typescript">function Update(deltaTime: float)</code></pre>
> Evaluates the animator based on deltaTime.
> 
> **Parameters**:
> - `deltaTime`: The time delta.
> 
<pre class="language-typescript"><code class="lang-typescript">function IsPlaying(anim: string, layer: int = 0) -> bool</code></pre>
> Checks if the given animation is playing.
> 
> **Parameters**:
> - `anim`: The name of the animation to check. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> - `layer`: The animation layer to check (default: 0).
> 
<pre class="language-typescript"><code class="lang-typescript">function IsTag(tag: string, layer: int = 0) -> bool</code></pre>
> Returns true if the current animation has the given tag.
> 
> **Parameters**:
> - `tag`: The name of the tag to check.
> - `layer`: The animation layer to check (default: 0).
> 
<pre class="language-typescript"><code class="lang-typescript">function GetTransitionDuration(layer: int = 0) -> float</code></pre>
> Gets the duration of the transition.
> 
> **Parameters**:
> - `layer`: The animation layer to check (default: 0).
> 
<pre class="language-typescript"><code class="lang-typescript">function GetTransitionNormalizedTime(layer: int = 0) -> float</code></pre>
> Gets the normalized time of the transition.
> 
> **Parameters**:
> - `layer`: The animation layer to check (default: 0).
> 
<pre class="language-typescript"><code class="lang-typescript">function PlayAnimation(anim: string, fade: float = 0.1, layer: int = 0)</code></pre>
> Plays the specified animation.
> 
> **Parameters**:
> - `anim`: The name of the animation to play. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> - `fade`: The fade time in seconds for cross-fading (default: 0.1).
> - `layer`: The animation layer to play on (default: 0).
> 
<pre class="language-typescript"><code class="lang-typescript">function PlayAnimationAt(anim: string, normalizedTime: float, fade: float = 0.1, layer: int = 0)</code></pre>
> Plays the specified animation starting from a normalized time.
> 
> **Parameters**:
> - `anim`: The name of the animation to play. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> - `normalizedTime`: The normalized time (0-1) to start the animation from.
> - `fade`: The fade time in seconds for cross-fading (default: 0.1).
> - `layer`: The animation layer to play on (default: 0).
> 
<pre class="language-typescript"><code class="lang-typescript">function SetSpeed(speed: float)</code></pre>
> Sets the animation playback speed.
> 
> **Parameters**:
> - `speed`: The playback speed multiplier (1.0 = normal speed).
> 
<pre class="language-typescript"><code class="lang-typescript">function GetAnimationLength(anim: string) -> float</code></pre>
> Gets the length of the specified animation.
> 
> **Parameters**:
> - `anim`: The name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function GetFloat(name: string) -> float</code></pre>
> Gets an animation float parameter.
> 
> **Parameters**:
> - `name`: The name of the float parameter.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetInteger(name: string) -> int</code></pre>
> Gets an animation int parameter.
> 
> **Parameters**:
> - `name`: The name of the int parameter.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetBool(name: string) -> bool</code></pre>
> Gets an animation bool parameter.
> 
> **Parameters**:
> - `name`: The name of the bool parameter.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetFloat(name: string, value: float)</code></pre>
> Sets an animation float parameter.
> 
> **Parameters**:
> - `name`: The name of the float parameter.
> - `value`: The value to set.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetInteger(name: string, value: int)</code></pre>
> Sets an animation int parameter.
> 
> **Parameters**:
> - `name`: The name of the int parameter.
> - `value`: The value to set.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetBool(name: string, value: bool)</code></pre>
> Sets an animation bool parameter.
> 
> **Parameters**:
> - `name`: The name of the bool parameter.
> - `value`: The value to set.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetTrigger(name: string)</code></pre>
> Sets an animation trigger.
> 
> **Parameters**:
> - `name`: The name of the trigger parameter.
> 
<pre class="language-typescript"><code class="lang-typescript">function ResetTrigger(name: string)</code></pre>
> Resets an animation trigger.
> 
> **Parameters**:
> - `name`: The name of the trigger parameter to reset.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetLayerWeight(layer: int, weight: float)</code></pre>
> Sets the weight of the specified layer.
> 
> **Parameters**:
> - `layer`: The layer index.
> - `weight`: The weight value (0-1) to set.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetLayerWeight(layer: int) -> float</code></pre>
> Gets the weight of the specified layer.
> 
> **Parameters**:
> - `layer`: The layer index.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetAnimationNormalizedTime(layer: int = 0) -> float</code></pre>
> Gets the normalized time of the current animation.
> 
> **Parameters**:
> - `layer`: The animation layer to check (default: 0).
> 

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
