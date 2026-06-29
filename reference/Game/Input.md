# Input
Inherits from [Object](../objects/Object.md)

Reading player key inputs. Note that inputs are best handled in OnFrame rather than OnTick,
due to being updated every frame and not every physics tick.

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function GetKeyName(key: string) -> string</code></pre>
> Gets the key name the player assigned to the key setting.
> 
> **Parameters**:
> - `key`: The key setting path (e.g., "General/Attack" or "CustomKey/Space"). Refer to [InputGeneralEnum](../Enums/InputGeneralEnum.md), [InputHumanEnum](../Enums/InputHumanEnum.md), [InputTitanEnum](../Enums/InputTitanEnum.md), [InputInteractionEnum](../Enums/InputInteractionEnum.md), [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md), [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
> 
> **Returns**: The key name.
<pre class="language-typescript"><code class="lang-typescript">function GetKeyHold(key: string) -> bool</code></pre>
> Returns true if the key is being held down.
> 
> **Parameters**:
> - `key`: The key setting path (e.g., "General/Attack" or "CustomKey/Space"). Refer to [InputGeneralEnum](../Enums/InputGeneralEnum.md), [InputHumanEnum](../Enums/InputHumanEnum.md), [InputTitanEnum](../Enums/InputTitanEnum.md), [InputInteractionEnum](../Enums/InputInteractionEnum.md), [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md), [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
> 
> **Returns**: True if the key is being held down, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function GetKeyDown(key: string) -> bool</code></pre>
> Returns true if the key was pressed down this frame.
> 
> **Parameters**:
> - `key`: The key setting path (e.g., "General/Attack" or "CustomKey/Space"). Refer to [InputGeneralEnum](../Enums/InputGeneralEnum.md), [InputHumanEnum](../Enums/InputHumanEnum.md), [InputTitanEnum](../Enums/InputTitanEnum.md), [InputInteractionEnum](../Enums/InputInteractionEnum.md), [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md), [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
> 
> **Returns**: True if the key was pressed down this frame, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function GetKeyUp(key: string) -> bool</code></pre>
> Returns true if the key was released this frame.
> 
> **Parameters**:
> - `key`: The key setting path (e.g., "General/Attack" or "CustomKey/Space"). Refer to [InputGeneralEnum](../Enums/InputGeneralEnum.md), [InputHumanEnum](../Enums/InputHumanEnum.md), [InputTitanEnum](../Enums/InputTitanEnum.md), [InputInteractionEnum](../Enums/InputInteractionEnum.md), [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md), [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
> 
> **Returns**: True if the key was released this frame, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function GetMouseAim() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Returns the position the player is aiming at.
> 
> **Returns**: The aim position.
<pre class="language-typescript"><code class="lang-typescript">function GetCursorAimDirection() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Returns the ray the player is aiming at.
> 
> **Returns**: The aim direction vector.
<pre class="language-typescript"><code class="lang-typescript">function GetMouseSpeed() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Returns the speed of the mouse.
> 
> **Returns**: The mouse speed vector.
<pre class="language-typescript"><code class="lang-typescript">function GetMousePosition() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Returns the position of the mouse.
> 
> **Returns**: The mouse position.
<pre class="language-typescript"><code class="lang-typescript">function GetScreenDimensions() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Returns the dimensions of the screen.
> 
> **Returns**: The screen dimensions.
<pre class="language-typescript"><code class="lang-typescript">function SetKeyDefaultEnabled(key: string, enabled: bool)</code></pre>
> Sets whether the key is enabled by default.
> 
> **Parameters**:
> - `key`: The key setting path (e.g., "General/Attack" or "CustomKey/Space"). Refer to [InputGeneralEnum](../Enums/InputGeneralEnum.md), [InputHumanEnum](../Enums/InputHumanEnum.md), [InputTitanEnum](../Enums/InputTitanEnum.md), [InputInteractionEnum](../Enums/InputInteractionEnum.md), [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md), [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
> - `enabled`: Whether the key should be enabled by default.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetKeyHold(key: string, enabled: bool)</code></pre>
> Sets whether the key is being held down.
> 
> **Parameters**:
> - `key`: The key setting path (e.g., "General/Attack" or "CustomKey/Space"). Refer to [InputGeneralEnum](../Enums/InputGeneralEnum.md), [InputHumanEnum](../Enums/InputHumanEnum.md), [InputTitanEnum](../Enums/InputTitanEnum.md), [InputInteractionEnum](../Enums/InputInteractionEnum.md), [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md), [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
> - `enabled`: Whether the key should be held down.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetCategoryKeysEnabled(category: string, enabled: bool)</code></pre>
> Sets whether all keys in the specified category are enabled by default.
> 
> **Parameters**:
> - `category`: The category name. Refer to [InputCategoryEnum](../Enums/InputCategoryEnum.md)
> - `enabled`: Whether the keys should be enabled by default.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetGeneralKeysEnabled(enabled: bool)</code></pre>
> Sets whether all General category keys are enabled by default.
> 
> **Parameters**:
> - `enabled`: Whether the keys should be enabled by default.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetInteractionKeysEnabled(enabled: bool)</code></pre>
> Sets whether all Interaction category keys are enabled by default.
> 
> **Parameters**:
> - `enabled`: Whether the keys should be enabled by default.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetTitanKeysEnabled(enabled: bool)</code></pre>
> Sets whether all Titan category keys are enabled by default.
> 
> **Parameters**:
> - `enabled`: Whether the keys should be enabled by default.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetHumanKeysEnabled(enabled: bool)</code></pre>
> Sets whether all Human category keys are enabled by default.
> 
> **Parameters**:
> - `enabled`: Whether the keys should be enabled by default.
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
