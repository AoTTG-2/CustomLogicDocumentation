# Shifter
Inherits from [Character](../Entities/Character.md)

Represents a Shifter character. Only character owner can modify fields and call functions unless otherwise specified.

### Example
```csharp
function OnCharacterSpawn(character)
{
    if (character.IsMine && character.Type == "Shifter")
    {
        character.Size = 2;
        if (Network.MyPlayer.Status == "Alive" && Network.MyPlayer.Character.Type == "Human")
        {
            character.Target(Network.MyPlayer, 10);
        }
    }
}
```
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Size|float|False|Shifter's size.|
|RunSpeedBase|float|False|Shifter's base run speed. Final run speed is RunSpeedBase + Size * RunSpeedPerLevel.|
|WalkSpeedBase|float|False|Shifter's base walk speed. Final walk speed is WalkSpeedBase + Size * WalkSpeedPerLevel.|
|WalkSpeedPerLevel|float|False|Shifter's walk speed added per level.|
|RunSpeedPerLevel|float|False|Shifter's run speed added per level.|
|TurnSpeed|float|False|Shifter's turn speed when running turn animation.|
|RotateSpeed|float|False|Shifter's rotate speed when rotating body.|
|JumpForce|float|False|Shifter's jump force when jumping.|
|ActionPause|float|False|Shifter's pause delay after performing an action.|
|AttackPause|float|False|Shifter's pause delay after performing an attack.|
|TurnPause|float|False|Shifter's pause delay after performing a turn.|
|DetectRange|float|False|(AI) shifter's detect range.|
|FocusRange|float|False|(AI) shifter's focus range.|
|FocusTime|float|False|(AI) shifter's focus time before switching targets.|
|FarAttackCooldown|float|False|(AI) Shifter's cooldown after performing a ranged attack.|
|AttackWait|float|False|(AI) Shifter's wait time between being in range to attack and performing the attack.|
|AttackSpeedMultiplier|float|False|Shifter's attack animation speed.|
|UsePathfinding|bool|False|(AI) Shifter uses pathfinding.|
|AIEnabled|bool|False|Enable/Disable AI Behavior (Shifter will not attack/target but pathfinding/move methods will still work).|
|NapePosition|[Vector3](../Collections/Vector3.md)|True|The shifter's nape position.|
|DeathAnimLength|float|False|The length of the death animation.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function MoveTo(position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, range: float, ignoreEnemies: bool)</code></pre>
> Causes the (AI) shifter to move towards a position. If ignoreEnemies is true, will not engage enemies along the way.
> 
> **Parameters**:
> - `position`: The target position to move to.
> - `range`: The stopping range from the target position.
> - `ignoreEnemies`: If true, will not engage enemies along the way.
> 
<pre class="language-typescript"><code class="lang-typescript">function MoveToExact(position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, timeoutPadding: float = 1)</code></pre>
> Causes the (AI) shifter to move towards a position. If ignoreEnemies is true, will not engage enemies along the way.
> 
> **Parameters**:
> - `position`: The exact target position to move to.
> - `timeoutPadding`: The timeout padding in seconds (default: 1).
> 
<pre class="language-typescript"><code class="lang-typescript">function MoveToExactCallback(method: function, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, range: float = 10, timeoutPadding: float = 1)</code></pre>
> Causes the (AI) shifter to move towards a position with a callback. The callback method will be called during movement and will receive this shifter as a parameter.
> 
> **Parameters**:
> - `method`: The callback method to call during movement (receives this shifter as parameter).
> - `position`: The exact target position to move to.
> - `range`: The stopping range from the target position (default: 10).
> - `timeoutPadding`: The timeout padding in seconds (default: 1).
> 
<pre class="language-typescript"><code class="lang-typescript">function Target(enemyObj: <a data-footnote-ref href="#user-content-fn-124">Object</a>, focus: float)</code></pre>
> Causes the (AI) shifter to target an enemy character or MapTargetable for focusTime seconds. If focusTime is 0 it will use the default focus time.
> 
> **Parameters**:
> - `enemyObj`: The enemy to target (can be Character or MapTargetable).
> - `focus`: The focus time in seconds (0 uses default focus time).
> 
<pre class="language-typescript"><code class="lang-typescript">function Idle(time: float)</code></pre>
> Causes the (AI) shifter to idle for time seconds before beginning to wander. During idle the titan will not react or move at all.
> 
> **Parameters**:
> - `time`: The idle time in seconds.
> 
<pre class="language-typescript"><code class="lang-typescript">function Wander()</code></pre>
> Causes the (AI) shifter to cancel any move commands and begin wandering randomly.
> 
<pre class="language-typescript"><code class="lang-typescript">function Blind()</code></pre>
> Causes the shifter to enter the blind state.
> 
<pre class="language-typescript"><code class="lang-typescript">function Cripple(time: float)</code></pre>
> Causes the shifter to enter the cripple state.
> 
> **Parameters**:
> - `time`: The cripple duration in seconds.
> 
<pre class="language-typescript"><code class="lang-typescript">function Attack(attack: string)</code></pre>
> Causes the shifter to perform the given attack, if able.
> 
> **Parameters**:
> - `attack`: The name of the attack to perform.
> 

### Hierarchy
**Annie**
```
Annie
├── Armature_FemT
│   └── Core
│       ├── Config
│       │   └── Config_end
│       ├── Controller_Body
│       │   └── hip
│       │       ├── spine
│       │       │   └── chest
│       │       │       ├── neck
│       │       │       │   ├── head
│       │       │       │   │   ├── Bone
│       │       │       │   │   │   ├── Bone_end
│       │       │       │   │   │   └── MouthHitbox
│       │       │       │   │   ├── hair_back
│       │       │       │   │   │   └── hair_back_end
│       │       │       │   │   ├── hair_front
│       │       │       │   │   │   └── hair_front_end
│       │       │       │   │   ├── hair_left
│       │       │       │   │   │   └── hair_left_end
│       │       │       │   │   ├── hair_right
│       │       │       │   │   │   └── hair_right_end
│       │       │       │   │   └── EyesHurtbox
│       │       │       │   └── NapeHurtbox
│       │       │       ├── shoulder_L
│       │       │       │   └── upper_arm_L
│       │       │       │       └── forearm_L
│       │       │       │           └── hand_L
│       │       │       │               ├── hand_L_001
│       │       │       │               │   └── hand_L_002
│       │       │       │               │       ├── hand_L_003
│       │       │       │               │       │   └── hand_L_003_end
│       │       │       │               │       └── HandLHitbox
│       │       │       │               └── hand_L_004
│       │       │       │                   └── hand_L_005
│       │       │       │                       └── hand_L_006
│       │       │       │                           └── hand_L_006_end
│       │       │       └── shoulder_R
│       │       │           └── upper_arm_R
│       │       │               └── forearm_R
│       │       │                   └── hand_R
│       │       │                       ├── hand_R_001
│       │       │                       │   ├── hand_R_002
│       │       │                       │   │   └── hand_R_003
│       │       │                       │   │       └── hand_R_003_end
│       │       │                       │   └── HandRHitbox
│       │       │                       └── hand_R_004
│       │       │                           └── hand_R_005
│       │       │                               └── hand_R_006
│       │       │                                   └── hand_R_006_end
│       │       ├── thigh_L
│       │       │   └── shin_L
│       │       │       ├── foot_L
│       │       │       │   └── toe_L
│       │       │       │       └── toe_L_end
│       │       │       ├── LegLHurtbox
│       │       │       └── FootLHitbox
│       │       └── thigh_R
│       │           └── shin_R
│       │               ├── foot_R
│       │               │   └── toe_R
│       │               │       └── toe_R_end
│       │               ├── LegRHurtbox
│       │               └── FootRHitbox
│       ├── HeadIK
│       │   └── HeadIK_end
│       ├── IK_L
│       │   └── knee_L
│       │       └── knee_L_end
│       └── IK_R
│           └── knee_R
│               └── knee_R_end
├── FemT
└── FemTHair
```

**Armored**
```
Armored
├── Amarture_VER2
│   └── Core
│       ├── Configure
│       ├── Controller.Body
│       │   └── hip
│       │       ├── spine
│       │       │   └── chest
│       │       │       ├── neck
│       │       │       │   └── head
│       │       │       │       └── Bone
│       │       │       ├── NapeHurtbox
│       │       │       ├── shoulder.L
│       │       │       │   └── upper_arm.L
│       │       │       │       └── forearm.L
│       │       │       │           └── hand.L
│       │       │       │               ├── hand.L.001
│       │       │       │               │   ├── hand.L.002
│       │       │       │               │   │   └── hand.L.003
│       │       │       │               │   └── HandLHitbox
│       │       │       │               └── hand.L.004
│       │       │       │                   └── hand.L.005
│       │       │       │                       └── hand.L.006
│       │       │       └── shoulder.R
│       │       │           └── upper_arm.R
│       │       │               └── forearm.R
│       │       │                   └── hand.R
│       │       │                       ├── hand.R.001
│       │       │                       │   ├── hand.R.002
│       │       │                       │   │   └── hand.R.003
│       │       │                       │   └── HandRHitbox
│       │       │                       └── hand.R.004
│       │       │                           └── hand.R.005
│       │       │                               └── hand.R.006
│       │       ├── thigh.L
│       │       │   └── shin.L
│       │       │       └── foot.L
│       │       │           └── toe.L
│       │       └── thigh.R
│       │           └── shin.R
│       │               └── foot.R
│       │                   └── toe.R
│       ├── Controller.Leg.L
│       │   ├── Controller.asset.foot.IK.L.002
│       │   │   └── Controller.asset.foot.IK.L.001
│       │   │       └── Controller.foot.IK.L
│       │   │           └── kneel.L
│       │   └── Controller.Foot.L
│       ├── Controller.Leg.R
│       │   ├── Controller.asset.foot.IK.R.002
│       │   │   └── Controller.asset.foot.IK.R.001
│       │   │       └── Controller.foot.IK.R
│       │   │           └── kneel.R
│       │   └── Controller.Foot.R
│       ├── IK_ElbowController.L
│       ├── IK_ElbowController.R
│       ├── IK_HandController.L
│       │   └── BridgeHand.L
│       └── IK_HandController.R
│           └── BridgeHand.R
├── def_titan
├── def_titan_hair
└── Anchor
```

**Eren**
```
Eren
├── ErenRig_VER2
│   └── Core
│       ├── ARM_IK_R
│       ├── Controller_Body
│       │   └── hip
│       │       ├── spine
│       │       │   └── chest
│       │       │       ├── neck
│       │       │       │   └── head
│       │       │       │       ├── Bone
│       │       │       │       ├── Bone_001
│       │       │       │       ├── Bone_002
│       │       │       │       └── Bone_003
│       │       │       ├── NapeHurtbox
│       │       │       ├── shoulder_L
│       │       │       │   └── upper_arm_L
│       │       │       │       └── forearm_L
│       │       │       │           └── hand_L
│       │       │       │               ├── hand_L_001
│       │       │       │               │   └── hand_L_002
│       │       │       │               │       └── hand_L_003
│       │       │       │               ├── HandLHitbox
│       │       │       │               └── hand_L_004
│       │       │       │                   └── hand_L_005
│       │       │       │                       └── hand_L_006
│       │       │       └── shoulder_R
│       │       │           └── upper_arm_R
│       │       │               └── forearm_R
│       │       │                   └── hand_R
│       │       │                       ├── hand_R_001
│       │       │                       │   └── hand_R_002
│       │       │                       │       └── hand_R_003
│       │       │                       ├── HandRHitbox
│       │       │                       └── hand_R_004
│       │       │                           └── hand_R_005
│       │       │                               └── hand_R_006
│       │       ├── thigh_L
│       │       │   └── shin_L
│       │       │       └── foot_L
│       │       │           ├── toe_L
│       │       │           └── FootLHitbox
│       │       └── thigh_R
│       │           └── shin_R
│       │               └── foot_R
│       │                   ├── toe_R
│       │                   └── FootRHitbox
│       ├── IK.L
│       │   └── kneel.L
│       ├── IK.R
│       │   └── kneel.R
│       ├── IK_ELBOW_R
│       ├── IK_TARGET
│       └── Rock
├── ErenTitan
└── ErenTitanHair
```

**WallColossal**
```
WallColossal
├── Armature_VER2
│   └── Core
│       ├── Controller_Body
│       │   └── hip
│       │       ├── spine
│       │       │   ├── abs
│       │       │   │   └── abs_end
│       │       │   └── chest
│       │       │       ├── breast.L
│       │       │       │   └── breast.L_end
│       │       │       ├── breast.R
│       │       │       │   └── breast.R_end
│       │       │       └── upperchest
│       │       │           ├── neck
│       │       │           │   ├── head
│       │       │           │   │   └── Bone
│       │       │           │   │       └── Bone_end
│       │       │           │   ├── NapeHurtbox
│       │       │           │   ├── ColossalSteam1
│       │       │           │   │   └── extra
│       │       │           │   ├── ColossalSteam2
│       │       │           │   │   ├── extra
│       │       │           │   │   └── embers
│       │       │           │   └── SteamHitbox
│       │       │           ├── shoulder_L
│       │       │           │   └── upper_arm_L
│       │       │           │       └── forearm_L
│       │       │           │           ├── hand_L
│       │       │           │           │   ├── hand_L_001.L
│       │       │           │           │   │   └── hand_L_001.001.L
│       │       │           │           │   │       └── hand_L_001.002.L
│       │       │           │           │   │           └── hand_L_001.002.L_end
│       │       │           │           │   ├── hand_L_004.L
│       │       │           │           │   │   └── hand_L_004.001.L
│       │       │           │           │   │       └── hand_L_004.002.L
│       │       │           │           │   │           └── hand_L_004.002.L_end
│       │       │           │           │   ├── hand_L_007.L
│       │       │           │           │   │   └── hand_L_007.001.L
│       │       │           │           │   │       └── hand_L_007.002.L
│       │       │           │           │   │           └── hand_L_007.002.L_end
│       │       │           │           │   ├── hand_L_011.L
│       │       │           │           │   │   └── hand_L_011.001.L
│       │       │           │           │   │       └── hand_L_011.002.L
│       │       │           │           │   │           └── hand_L_011.002.L_end
│       │       │           │           │   ├── hand_L_013.L
│       │       │           │           │   │   └── hand_L_013.001.L
│       │       │           │           │   │       └── hand_L_013.002.L
│       │       │           │           │   │           └── hand_L_013.002.L_end
│       │       │           │           │   ├── HandLHitbox
│       │       │           │           │   └── HandLHurtbox
│       │       │           │           ├── ForearmLHitbox
│       │       │           │           └── ArmSmokeParticle
│       │       │           │               └── Particle System
│       │       │           ├── shoulder_R
│       │       │           │   └── upper_arm_R
│       │       │           │       └── forearm_R
│       │       │           │           ├── hand_R
│       │       │           │           │   ├── hand_L_001.R
│       │       │           │           │   │   └── hand_L_001.001.R
│       │       │           │           │   │       └── hand_L_001.002.R
│       │       │           │           │   │           └── hand_L_001.002.R_end
│       │       │           │           │   ├── hand_L_004.R
│       │       │           │           │   │   └── hand_L_004.001.R
│       │       │           │           │   │       └── hand_L_004.002.R
│       │       │           │           │   │           └── hand_L_004.002.R_end
│       │       │           │           │   ├── hand_L_007.R
│       │       │           │           │   │   └── hand_L_007.001.R
│       │       │           │           │   │       └── hand_L_007.002.R
│       │       │           │           │   │           └── hand_L_007.002.R_end
│       │       │           │           │   ├── hand_L_011.R
│       │       │           │           │   │   └── hand_L_011.001.R
│       │       │           │           │   │       └── hand_L_011.002.R
│       │       │           │           │   │           └── hand_L_011.002.R_end
│       │       │           │           │   ├── hand_L_013.R
│       │       │           │           │   │   └── hand_L_013.001.R
│       │       │           │           │   │       └── hand_L_013.002.R
│       │       │           │           │   │           └── hand_L_013.002.R_end
│       │       │           │           │   ├── HandRHitbox
│       │       │           │           │   └── HandRHurtbox
│       │       │           │           ├── ForearmRHitbox
│       │       │           │           └── ArmSmokeParticle
│       │       │           │               └── Particle System
│       │       │           ├── breastpushbox
│       │       │           ├── breastanglepushbox
│       │       │           └── upperchestpushbox
│       │       ├── thigh_L
│       │       │   └── shin_L
│       │       │       └── foot_L
│       │       │           ├── toe.L
│       │       │           │   └── toe.L_end
│       │       │           └── FootLHitbox
│       │       └── thigh_R
│       │           └── shin_R
│       │               └── foot_R
│       │                   ├── toe.R
│       │                   │   └── toe.R_end
│       │                   └── FootRHitbox
│       ├── IK.L
│       │   └── knee.L
│       │       └── knee.L_end
│       ├── IK.R
│       │   └── knee.R
│       │       └── knee.R_end
│       ├── IK_hand_L
│       │   ├── IK_Elbow_L
│       │   │   └── IK_Elbow_L_end
│       │   └── IK_stable_L
│       │       └── IK_stable_L_end
│       └── IK_hand_R
│           ├── IK_Elbow_R
│           │   └── IK_Elbow_R_end
│           └── IK_stable_R
│               └── IK_stable_R_end
└── Colossal_VER2
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
