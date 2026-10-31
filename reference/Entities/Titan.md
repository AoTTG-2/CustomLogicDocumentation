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
|DeathType|int|False|Refer to [TitanDeathTypeEnum](../Enums/TitanDeathTypeEnum.md)|
|DeathVelocity|[Vector3](../Collections/Vector3.md)|False||
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
|IsWarded|bool|False|Whether the titan has the warded modifier. Setting this changes the warded state for all clients.|
|IsHardened|bool|True|Whether the titan's nape is currently hardened. Breaking the warded weak spot temporarily removes hardening.|
|FocusRange|float|False|(AI) titan's focus range.|
|FocusTime|float|False|(AI) default target focus time in seconds.|
|FarAttackCooldown|float|False|(AI) Titan's cooldown after performing a ranged attack.|
|AttackWait|float|False|(AI) Titan's wait time between being in range and performing an attack.|
|CanRun|bool|False|(AI) Titan can run or only walk.|
|AttackSpeedMultiplier|float|False|Titan's attack animation speed.|
|HeadMount|[Transform](../Entities/Transform.md)|True|Titan's head transform.|
|NeckMount|[Transform](../Entities/Transform.md)|True|Titan's neck transform.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Wander()</code></pre>
> Cancels (AI) movement and targeting, then resumes normal AI behavior.
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
<pre class="language-typescript"><code class="lang-typescript">function Stun(duration: float = 0)</code></pre>
> Stuns the titan.
> 
> **Parameters**:
> - `duration`: Stun time in seconds. 0 uses the default.
> 
<pre class="language-typescript"><code class="lang-typescript">function Target(enemyObj: <a data-footnote-ref href="#user-content-fn-127">Object</a>, focus: float)</code></pre>

{% hint style="warning" %}
**Obsolete**: Use SetTarget(target, focusDuration) instead.
{% endhint %}

> (AI) alias for SetTarget(enemyObj, focus).
> 
> **Parameters**:
> - `enemyObj`: A Character or MapTargetable, or null.
> - `focus`: Focus time in seconds. 0 uses FocusTime.
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
│       │   │   │       │   ├── NapeHurtbox
│       │   │   │       │   ├── Momo_HardenedNapePF
│       │   │   │       │   └── NeckPushbox
│       │   │   │       ├── shoulder.L
│       │   │   │       │   └── upper_arm.L
│       │   │   │       │       ├── forearm.L
│       │   │   │       │       │   ├── hand.L
│       │   │   │       │       │   │   ├── hand.L.001
│       │   │   │       │       │   │   │   ├── hand.L.002
│       │   │   │       │       │   │   │   │   └── hand.L.003
│       │   │   │       │       │   │   │   │       └── hand.L.003_end
│       │   │   │       │       │   │   │   ├── HandLHitbox
│       │   │   │       │       │   │   │   └── HandLHurtbox
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
│       │   │   │               │   │   │   ├── HandRHitbox
│       │   │   │               │   │   │   └── HandRHurtbox
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
