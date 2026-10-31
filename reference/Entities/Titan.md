# Titan
Inherits from [Character](../Entities/Character.md)

Represents a Titan character. Only character owner can modify fields and call functions unless otherwise specified.

### Example
```csharp
function OnCharacterSpawn(character)
{
    if (character.IsMine && character.Type == "Titan")
    {
        character.Size = 3;
        character.DetectRange = 1000;
        character.Blind();
    }
}
```
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Size|float|False|Titan's size.|
|HeadSize|float|False|Titan's head size scaling relative to its Size. This is set locally by the client. This value is reset when the titan's Size is changed.|
|RunSpeedBase|float|False|Titan's base run speed. Final run speed is RunSpeedBase + Size * RunSpeedPerLevel.|
|WalkSpeedBase|float|False|Titan's base walk speed. Final walk speed is WalkSpeedBase + Size * WalkSpeedPerLevel.|
|WalkSpeedPerLevel|float|False|Titan's walk speed added per size.|
|RunSpeedPerLevel|float|False|Titan's run speed added per size.|
|TurnSpeed|float|False|Titan's turn animation speed.|
|RotateSpeed|float|False|Titan's rotate speed.|
|JumpForce|float|False|Titan's jump force.|
|ActionPause|float|False|Titan's pause delay after performing an action.|
|AttackPause|float|False|Titan's pause delay after performing an attack.|
|TurnPause|float|False|Titan's pause delay after performing a turn.|
|Stamina|float|False|PT stamina.|
|MaxStamina|float|False|PT max stamina.|
|NapePosition|[Vector3](../Collections/Vector3.md)|True|The titan's nape position.|
|IsCrawler|bool|True|Is titan a crawler.|
|State|string|True|State of the titan.|
|DetectRange|float|False|(AI) titan's detect range.|
|FocusRange|float|False|(AI) titan's focus range.|
|FocusTime|float|False|(AI) titan's focus time.|
|FarAttackCooldown|float|False|(AI) Titan's cooldown after performing a ranged attack.|
|AttackWait|float|False|(AI) Titan's wait time between being in range and performing an attack.|
|CanRun|bool|False|(AI) Titan can run or only walk.|
|AttackSpeedMultiplier|float|False|Titan's attack animation speed.|
|UsePathfinding|bool|False|Determines whether the (AI) titan uses pathfinding. (Smart Movement in titan settings)|
|HeadMount|[Transform](../Entities/Transform.md)|True|Titan's head transform.|
|NeckMount|[Transform](../Entities/Transform.md)|True|Titan's neck transform.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function MoveTo(position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, range: float, ignoreEnemies: bool)</code></pre>
> Causes the (AI) titan to move towards a position and stopping when within specified range. If ignoreEnemies is true, will not engage enemies along the way.
> 
> **Parameters**:
> - `position`: The target position to move to.
> - `range`: The stopping range from the target position.
> - `ignoreEnemies`: If true, will not engage enemies along the way.
> 
<pre class="language-typescript"><code class="lang-typescript">function Target(enemyObj: <a data-footnote-ref href="#user-content-fn-124">Object</a>, focus: float)</code></pre>
> Causes the (AI) titan to target an enemy character or MapTargetable for focusTime seconds. If focusTime is 0 it will use the default focus time.
> 
> **Parameters**:
> - `enemyObj`: The enemy to target (can be Character or MapTargetable).
> - `focus`: The focus time in seconds (0 uses default focus time).
> 
<pre class="language-typescript"><code class="lang-typescript">function GetTarget() -> <a data-footnote-ref href="#user-content-fn-124">Object</a></code></pre>
> Gets the target currently focused by this character.
> 
> **Returns**: Returns null if no target is set.
<pre class="language-typescript"><code class="lang-typescript">function Idle(time: float)</code></pre>
> Causes the (AI) titan to idle for time seconds before beginning to wander. During idle the titan will not react or move at all.
> 
> **Parameters**:
> - `time`: The idle time in seconds.
> 
<pre class="language-typescript"><code class="lang-typescript">function Wander()</code></pre>
> Causes the (AI) titan to cancel any move commands and begin wandering randomly.
> 
<pre class="language-typescript"><code class="lang-typescript">function Blind()</code></pre>
> Causes the titan to enter the blind state.
> 
<pre class="language-typescript"><code class="lang-typescript">function Cripple(time: float)</code></pre>
> Causes the titan to enter the cripple state for time seconds. Using 0 will use the default cripple time.
> 
> **Parameters**:
> - `time`: The cripple duration in seconds (0 uses default time).
> 

### Hierarchy
**BasicTitan0**
```
BasicTitan0
├── Amarture_VER2
│   └── Core
│       ├── CrawlerHitbox
│       │   └── Cube
│       ├── Configure
│       │   └── Configure_end
│       ├── Controller.Body
│       │   ├── hip
│       │   │   ├── spine
│       │   │   │   └── chest
│       │   │   │       ├── neck
│       │   │   │       │   ├── head
│       │   │   │       │   │   ├── Bone
│       │   │   │       │   │   │   └── MouthHitbox
│       │   │   │       │   │   ├── HairSocket
│       │   │   │       │   │   ├── EyesHurtbox
│       │   │   │       │   │   └── Eyes
│       │   │   │       │   └── NapeHurtbox
│       │   │   │       ├── shoulder.L
│       │   │   │       │   └── upper_arm.L
│       │   │   │       │       ├── forearm.L
│       │   │   │       │       │   ├── hand.L
│       │   │   │       │       │   │   ├── hand.L.001
│       │   │   │       │       │   │   │   ├── hand.L.002
│       │   │   │       │       │   │   │   │   └── hand.L.003
│       │   │   │       │       │   │   │   │       └── hand.L.003_end
│       │   │   │       │       │   │   │   └── HandLHitbox
│       │   │   │       │       │   │   ├── hand.L.004
│       │   │   │       │       │   │   │   └── hand.L.005
│       │   │   │       │       │   │   │       └── hand.L.006
│       │   │   │       │       │   │   │           └── hand.L.006_end
│       │   │   │       │       │   │   └── GrabLSocket
│       │   │   │       │       │   ├── Forearm_Col_L
│       │   │   │       │       │   └── ForearmLHurtbox
│       │   │   │       │       └── Arm_Col_L
│       │   │   │       └── shoulder.R
│       │   │   │           └── upper_arm.R
│       │   │   │               ├── forearm.R
│       │   │   │               │   ├── hand.R
│       │   │   │               │   │   ├── hand.R.001
│       │   │   │               │   │   │   ├── hand.R.002
│       │   │   │               │   │   │   │   └── hand.R.003
│       │   │   │               │   │   │   │       └── hand.R.003_end
│       │   │   │               │   │   │   └── HandRHitbox
│       │   │   │               │   │   ├── hand.R.004
│       │   │   │               │   │   │   └── hand.R.005
│       │   │   │               │   │   │       └── hand.R.006
│       │   │   │               │   │   │           └── hand.R.006_end
│       │   │   │               │   │   └── GrabRSocket
│       │   │   │               │   ├── Forearm_Col_R
│       │   │   │               │   └── ForearmRHurtbox
│       │   │   │               └── Arm_Col_R
│       │   │   ├── thigh.L
│       │   │   │   ├── shin.L
│       │   │   │   │   ├── foot.L
│       │   │   │   │   │   ├── toe.L
│       │   │   │   │   │   │   └── toe.L_end
│       │   │   │   │   │   └── FootLHitbox
│       │   │   │   │   ├── LegLHurtbox
│       │   │   │   │   └── Shin_Col_L
│       │   │   │   └── Thigh_Col_L
│       │   │   └── thigh.R
│       │   │       ├── shin.R
│       │   │       │   ├── foot.R
│       │   │       │   │   ├── toe.R
│       │   │       │   │   │   └── toe.R_end
│       │   │       │   │   └── FootRHitbox
│       │   │       │   ├── Shin_Col_R
│       │   │       │   └── LegRHurtbox
│       │   │       └── Thigh_Col_R
│       │   ├── BodyHitbox
│       │   │   └── Cube
│       │   └── SitPushbox
│       ├── Controller.Leg.L
│       │   ├── Controller.asset.foot.IK.L.002
│       │   │   └── Controller.asset.foot.IK.L.001
│       │   │       └── Controller.foot.IK.L
│       │   │           └── kneel.L
│       │   │               └── kneel.L_end
│       │   └── Controller.Foot.L
│       │       └── Controller.Foot.L_end
│       ├── Controller.Leg.R
│       │   ├── Controller.asset.foot.IK.R.002
│       │   │   └── Controller.asset.foot.IK.R.001
│       │   │       └── Controller.foot.IK.R
│       │   │           └── kneel.R
│       │   │               └── kneel.R_end
│       │   └── Controller.Foot.R
│       │       └── Controller.Foot.R_end
│       ├── IK_ElbowController.L
│       │   └── IK_ElbowController.L_end
│       ├── IK_ElbowController.R
│       │   └── IK_ElbowController.R_end
│       ├── IK_HandController.L
│       │   └── BridgeHand.L
│       │       └── BridgeHand.L_end
│       └── IK_HandController.R
│           └── BridgeHand.R
│               └── BridgeHand.R_end
├── Body
└── Head
```

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
[^82]: [TSKillSoundEnum](../Enums/TSKillSoundEnum.md)
[^83]: [TeamEnum](../Enums/TeamEnum.md)
[^84]: [TextAlignEnum](../Enums/TextAlignEnum.md)
[^85]: [TextOverflowEnum](../Enums/TextOverflowEnum.md)
[^86]: [TitanAnimationEnum](../Enums/TitanAnimationEnum.md)
[^87]: [TitanSoundEnum](../Enums/TitanSoundEnum.md)
[^88]: [TitanTypeEnum](../Enums/TitanTypeEnum.md)
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
