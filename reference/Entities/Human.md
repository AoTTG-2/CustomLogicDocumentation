# Human
Inherits from [Character](../Entities/Character.md)

Represents a human character. Only character owner can modify fields and call functions unless otherwise specified.

### Example
```csharp
function OnCharacterSpawn(character)
{
    if (character.IsMainCharacter && character.Type == "Human")
    {
        character.SetWeapon(WeaponEnum.Blade);
        character.SetSpecial(SpecialEnum.Potato);
        character.CurrentGas = character.MaxGas / 2;
    }
}
```
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Position|[Vector3](../Collections/Vector3.md)|False|Position of the character.|
|Weapon|string|False|The weapon the human is using. Refer to [WeaponEnum](../Enums/WeaponEnum.md)|
|CurrentSpecial|string|False|The current special the human is using. Refer to [SpecialEnum](../Enums/SpecialEnum.md)|
|SpecialCooldownTime|float|False|The normalized cooldown time of the special. Has a range of 0 to 1.|
|SpecialCooldown|float|False|The cooldown of the special.|
|ShifterLiveTime|float|False|The live time of the shifter special.|
|SpecialCooldownRatio|float|True|The ratio of the special cooldown.|
|CurrentGas|float|False|The current gas of the human.|
|MaxGas|float|False|The max gas of the human.|
|Acceleration|int|False|The acceleration of the human.|
|Speed|int|False|The speed of the human.|
|Horse|[Horse](../Entities/Horse.md)|True|The owner's horse, or null if unavailable.|
|HorseFollowEnabled|bool|False|Whether the horse follows this human.|
|HorseTransform|[Transform](../Entities/Transform.md)|True|The transform of the horse belonging to this human. Returns null if horses are disabled.|
|HorseSpeed|float|False|The speed of the horse.|
|CurrentBladeDurability|float|False|The current blade durability.|
|MaxBladeDurability|float|False|The max blade durability.|
|CurrentBlade|int|False|The current blade.|
|MaxBlade|int|False|The max number of blades held.|
|CurrentAmmoRound|int|False|The current ammo round.|
|MaxAmmoRound|int|False|The max ammo round.|
|CurrentAmmoLeft|int|False|The current ammo left.|
|MaxAmmoTotal|int|False|The max total ammo.|
|LeftHookEnabled|bool|False|Whether the left hook is enabled.|
|RightHookEnabled|bool|False|Whether the right hook is enabled.|
|IsMounted|bool|True|Whether the human is mounted.|
|MountState|int|True|The mount state of human. 0: None, 1: Horse, 2: MapObject.|
|MountedMapObject|[MapObject](../Entities/MapObject.md)|True|The map object the human is mounted on.|
|MountedTransform|[Transform](../Entities/Transform.md)|True|The transform the human is mounted on.|
|AutoRefillGas|bool|False|Whether the human auto refills gas.|
|CanDodge|bool|False|Whether the human can dodge.|
|IsInvincible|bool|False|Whether the human is invincible.|
|InvincibleTimeLeft|float|False|The time left for invincibility.|
|IsCarried|bool|True|If the human is carried.|
|Pivot|bool|True|If the human can hold reel in/out.|
|PivotPosition|[Vector3](../Collections/Vector3.md)|True|The position of the pivot when the human holds reel in/out.|
|IsHookedLeft|bool|True|If the left hook is hooked.|
|IsHookedRight|bool|True|If the right hook is hooked.|
|IsHookingLeft|bool|True|If the left hook is in the air.|
|IsHookingRight|bool|True|If the right hook is in the air.|
|HasHookLeft|bool|True|If the left hook is used.|
|HasHookRight|bool|True|If the right hook is used.|
|LeftHookReady|bool|True|If the left hook is ready.|
|RightHookReady|bool|True|If the right hook is ready.|
|LeftHookPosition|[Vector3](../Collections/Vector3.md)|True|Position of the left hook. Returns null if there is no hook.|
|RightHookPosition|[Vector3](../Collections/Vector3.md)|True|Position of the right hook. Returns null if there is no hook.|
|FocusRange|float|False|(AI) human's focus range.|
|FocusTime|float|False|(AI) default target focus time in seconds.|
|Target|[Object](../objects/Object.md)|False|**Obsolete**: Use GetTarget() and SetTarget() instead. (AI) target. Use GetTarget() and SetTarget() instead.|
|TargetPosition|[Vector3](../Collections/Vector3.md)|False|The movement or aiming target position of the (AI) human.|
|TargetVelocity|[Vector3](../Collections/Vector3.md)|True|The target velocity of the (AI) human.|
|AllowHorse|bool|False|Allow the (AI) human to have horse.|
|AllowSkin|bool|False|Allow the (AI) human to use the skin. (preset skin only)|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Refill() -> bool</code></pre>
> Refills the gas of the human.
> 
> **Returns**: True if refill was successful, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function RefillImmediate()</code></pre>
> Refills the gas of the human immediately.
> 
<pre class="language-typescript"><code class="lang-typescript">function ClearHooks()</code></pre>
> Clears all hooks.
> 
<pre class="language-typescript"><code class="lang-typescript">function ClearLeftHook()</code></pre>
> Clears the left hook.
> 
<pre class="language-typescript"><code class="lang-typescript">function ClearRightHook()</code></pre>
> Clears the right hook.
> 
<pre class="language-typescript"><code class="lang-typescript">function MountMapObject(mapObject: <a data-footnote-ref href="#user-content-fn-25">MapObject</a>, positionOffset: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationOffset: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, canMountedAttack: bool = False)</code></pre>
> Mounts the human on a map object.
> 
> **Parameters**:
> - `mapObject`: The map object to mount on.
> - `positionOffset`: The position offset from the mount point.
> - `rotationOffset`: The rotation offset from the mount point.
> - `canMountedAttack`: If true, allows the human to attack while mounted (default: false).
> 
<pre class="language-typescript"><code class="lang-typescript">function MountTransform(transform: <a data-footnote-ref href="#user-content-fn-31">Transform</a>, positionOffset: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationOffset: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, canMountedAttack: bool = False)</code></pre>
> Mounts the human on a transform.
> 
> **Parameters**:
> - `transform`: The transform to mount on.
> - `positionOffset`: The position offset from the mount point.
> - `rotationOffset`: The rotation offset from the mount point.
> - `canMountedAttack`: If true, allows the human to attack while mounted (default: false).
> 
<pre class="language-typescript"><code class="lang-typescript">function Unmount(immediate: bool = True)</code></pre>
> Unmounts the human.
> 
> **Parameters**:
> - `immediate`: If true, unmounts immediately without animation (default: true).
> 
<pre class="language-typescript"><code class="lang-typescript">function SetSpecial(special: string)</code></pre>
> Sets the special of the human.
> 
> **Parameters**:
> - `special`: The name of the special to set. Refer to [SpecialEnum](../Enums/SpecialEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function ActivateSpecial()</code></pre>
> Activates the special of the human.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetWeapon(weapon: string)</code></pre>
> Sets the weapon for the human.
> 
> **Parameters**:
> - `weapon`: Name of the weapon. Refer to [WeaponEnum](../Enums/WeaponEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function DisablePerks()</code></pre>
> Disables all perks of the human.
> 
<pre class="language-typescript"><code class="lang-typescript">function HasAIState(name: string) -> bool</code></pre>
> Determine whether an AIState exists for the (AI) human.
> 
> **Parameters**:
> - `name`: The name of the AI state.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetAIState(name: string, classInstance: UserClassInstance = null)</code></pre>
> (AI) registers or removes a custom AI state.
> 
> **Parameters**:
> - `name`: State name.
> - `classInstance`: State instance, or null to remove.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetAIState() -> string</code></pre>
> (AI) current AI state name, or null.
> 
<pre class="language-typescript"><code class="lang-typescript">function SwitchAIState(name: string)</code></pre>
> (AI) switches to a registered state.
> 
> **Parameters**:
> - `name`: State name.
> 
<pre class="language-typescript"><code class="lang-typescript">function ResetCallback(callback: string, method: function = null)</code></pre>
> (AI) sets or clears a callback.
> 
> **Parameters**:
> - `callback`: OnIdle, PreAction, PostAction, or MoveToCallback.
> - `method`: Method with no arguments, or null to clear.
> 
<pre class="language-typescript"><code class="lang-typescript">function Move(direction: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>)</code></pre>
> Causes the (AI) human to move.
> 
> **Parameters**:
> - `direction`: The direction to move in.
> 
<pre class="language-typescript"><code class="lang-typescript">function AimAt(position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>)</code></pre>
> Causes the (AI) human to aim at the specific position.
> 
> **Parameters**:
> - `position`: The position to aim at.
> 
<pre class="language-typescript"><code class="lang-typescript">function Jump()</code></pre>
> Causes the (AI) human to jump.
> 
<pre class="language-typescript"><code class="lang-typescript">function HorseMount(mount: bool = True)</code></pre>
> Causes the (AI) human to mount on their horse.
> 
> **Parameters**:
> - `mount`: True to mount, false to dismount.
> 
<pre class="language-typescript"><code class="lang-typescript">function Dodge()</code></pre>
> Causes the (AI) human to dodge.
> 
<pre class="language-typescript"><code class="lang-typescript">function Reload()</code></pre>
> Causes the (AI) human to reload.
> 
<pre class="language-typescript"><code class="lang-typescript">function UseGas(useGas: bool)</code></pre>
> Causes the (AI) human to use gas.
> 
> **Parameters**:
> - `useGas`: True to use gas, false to stop.
> 
<pre class="language-typescript"><code class="lang-typescript">function HorseWalk(isWalk: bool)</code></pre>
> Causes the (AI) human mounted on the horse to walk.
> 
> **Parameters**:
> - `isWalk`: True to walk, false to stop walking.
> 
<pre class="language-typescript"><code class="lang-typescript">function Dash(direction: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>)</code></pre>
> Causes the (AI) human to dash.
> 
> **Parameters**:
> - `direction`: The direction to dash in.
> 
<pre class="language-typescript"><code class="lang-typescript">function Reel(reelAxis: int)</code></pre>
> Causes the (AI) human to reel. -1 is reel in, 1 is reel out, 0 is not reel.
> 
> **Parameters**:
> - `reelAxis`: The reel axis value.
> 
<pre class="language-typescript"><code class="lang-typescript">function LaunchHookLeft(aimPoint: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>)</code></pre>
> Causes the (AI) human to launch the left hook.
> 
> **Parameters**:
> - `aimPoint`: The aim point for the hook.
> 
<pre class="language-typescript"><code class="lang-typescript">function LaunchHookRight(aimPoint: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>)</code></pre>
> Causes the (AI) human to launch the right hook.
> 
> **Parameters**:
> - `aimPoint`: The aim point for the hook.
> 
<pre class="language-typescript"><code class="lang-typescript">function ReleaseHookLeft()</code></pre>
> Causes the (AI) human to release the left hook.
> 
<pre class="language-typescript"><code class="lang-typescript">function ReleaseHookRight()</code></pre>
> Causes the (AI) human to release the right hook.
> 
<pre class="language-typescript"><code class="lang-typescript">function ReleaseHookAll()</code></pre>
> Causes the (AI) human to release all hooks.
> 
<pre class="language-typescript"><code class="lang-typescript">function Attack(attackOn: bool)</code></pre>
> Sends attack input to the (AI) human's weapon when its character state allows attacking.
> 
> **Parameters**:
> - `attackOn`: True to start attacking, false to stop.
> 
<pre class="language-typescript"><code class="lang-typescript">function Navigation()</code></pre>
> Updates the (AI) human's movement direction and magnitude towards TargetPosition, using pathfinding when enabled.
This performs one movement update; it does not create a movement order or check a stopping range.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetParticleEffect(effectName: string, enabled: bool)</code></pre>
> Enables or disables a particle effect.
> 
> **Parameters**:
> - `effectName`: Name of the effect. Refer to [HumanParticleEffectEnum](../Enums/HumanParticleEffectEnum.md)
> - `enabled`: True to enable, false to disable.
> 
<pre class="language-typescript"><code class="lang-typescript">function FindNearestEnemy()</code></pre>

{% hint style="warning" %}
**Obsolete**: Use TargetNearestEnemy() to assign or GetNearestEnemy() to query.
{% endhint %}

> Legacy enemy assignment for an (AI) human.
Use GetNearestEnemy() or TargetNearestEnemy() instead.
> 

### Hierarchy
**HumanPlayer**
```
HumanPlayer
├── Armature
│   └── Core
│       ├── PlayerWindTrailEffect
│       ├── Controller_Body
│       │   └── hip
│       │       ├── spine
│       │       │   └── chest
│       │       │       ├── neck
│       │       │       │   └── head
│       │       │       │       └── char_head
│       │       │       ├── shoulder_L
│       │       │       │   └── upper_arm_L
│       │       │       │       └── forearm_L
│       │       │       │           └── hand_L
│       │       │       │               ├── hookRef
│       │       │       │               └── checkBox
│       │       │       ├── shoulder_R
│       │       │       │   └── upper_arm_R
│       │       │       │       └── forearm_R
│       │       │       │           └── hand_R
│       │       │       │               ├── hookRef
│       │       │       │               └── checkBox
│       │       │       ├── hookRefR1
│       │       │       └── hookRefL1
│       │       ├── thigh_L
│       │       │   └── shin_L
│       │       │       └── foot_L
│       │       └── thigh_R
│       │           └── shin_R
│       │               └── foot_R
│       ├── IK_L
│       │   └── knee.L
│       └── IK_R
│           └── knee.R
├── 3dmg_smoke
├── speedFX
│   └── speedEffect
├── slideSparks
├── character_chest
├── character_leg
├── character_arm_l
├── character_arm_r
├── character_body
├── character_hand_l
├── character_hand_r
├── GroundRight
├── GroundLeft
├── buff1
│   ├── LeviSpinTest1
│   └── Particle System
├── buff2
└── fire1
    ├── Sparks
    └── SteamEffect
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
