# Player
Inherits from [Object](../objects/Object.md)

Represents a network player. Only master client or player may modify fields.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Character|[Character](../Entities/Character.md)|True|Player's current character, if alive.|
|Connected|bool|True|Player is still connected to the room.|
|ID|int|True|Player unique ID.|
|IsAnonymous|bool|True|Player is anonymous (no user ID).|
|UserID|string|True|Player unique user ID. Server sets this value authoritatively but locally players can still manipulate this. Read this property from your own host (masterclient) when using for identity.|
|Name|string|True|Player name.|
|DisplayName|string|True|Host-authoritative display name (server prop: display_name).|
|Guild|string|True|Player guild.|
|Team|string|True|Player's chosen team. Note that this may be different from the character's final team (Character.Team field) if the character's team field is modified. Refer to [TeamEnum](../Enums/TeamEnum.md)|
|Status|string|True|Player's spawn status. Refer to [PlayerStatusEnum](../Enums/PlayerStatusEnum.md)|
|CharacterType|string|True|Player's chosen character. Refer to [CharacterTypeEnum](../Enums/CharacterTypeEnum.md)|
|Loadout|string|True|Player's chosen loadout. Refer to [LoadoutEnum](../Enums/LoadoutEnum.md)|
|Kills|int|False|Player's kills.|
|Deaths|int|False|Player's deaths.|
|HighestDamage|int|False|Player's highest damage.|
|TotalDamage|int|False|Player's total damage.|
|Ping|int|True|The player's connection ping.|
|SpectateID|int|True|The player's spectating ID. If not spectating anyone, returns -1.|
|SpawnPoint|[Vector3](../Collections/Vector3.md)|False|Player's respawn point. Is initially null and can be set back to null, at which point map spawn points are used.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function GetCustomProperty(property: string) -> <a data-footnote-ref href="#user-content-fn-124">Object</a></code></pre>
> Get a custom property at given key. Must be a primitive type. This is synced to all clients.
> 
> **Parameters**:
> - `property`: The property key to get.
> 
> **Returns**: The property value.
<pre class="language-typescript"><code class="lang-typescript">function SetCustomProperty(property: string, value: <a data-footnote-ref href="#user-content-fn-124">Object</a>)</code></pre>
> Sets a custom property at given key. Must be a primitive type. This is synced to all clients.
> 
> **Parameters**:
> - `property`: The property key to set.
> - `value`: The value to set (must be a primitive type).
> 
<pre class="language-typescript"><code class="lang-typescript">function ClearKDR()</code></pre>
> Clears kills, deaths, highestdamage, and totaldamage properties.
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
[^95]: [Commands](../Game/Commands.md)
[^96]: [Cutscene](../Game/Cutscene.md)
[^97]: [Game](../Game/Game.md)
[^98]: [Input](../Game/Input.md)
[^99]: [Locale](../Game/Locale.md)
[^100]: [Map](../Game/Map.md)
[^101]: [Network](../Game/Network.md)
[^102]: [PersistentData](../Game/PersistentData.md)
[^103]: [Physics](../Game/Physics.md)
[^104]: [RoomData](../Game/RoomData.md)
[^105]: [Service](../Game/Service.md)
[^106]: [Time](../Game/Time.md)
[^107]: [Button](../UIElements/Button.md)
[^108]: [Dropdown](../UIElements/Dropdown.md)
[^109]: [Icon](../UIElements/Icon.md)
[^110]: [Image](../UIElements/Image.md)
[^111]: [Label](../UIElements/Label.md)
[^112]: [ProgressBar](../UIElements/ProgressBar.md)
[^113]: [ScrollView](../UIElements/ScrollView.md)
[^114]: [Slider](../UIElements/Slider.md)
[^115]: [TextField](../UIElements/TextField.md)
[^116]: [Toggle](../UIElements/Toggle.md)
[^117]: [UI](../UIElements/UI.md)
[^118]: [VisualElement](../UIElements/VisualElement.md)
[^119]: [Convert](../Utility/Convert.md)
[^120]: [Json](../Utility/Json.md)
[^121]: [Math](../Utility/Math.md)
[^122]: [Random](../Utility/Random.md)
[^123]: [String](../Utility/String.md)
[^124]: [Object](../objects/Object.md)
[^125]: [Component](../objects/Component.md)
