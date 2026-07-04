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
|HorseFollowEnabled|bool|False|Whether horse follow is enabled.|
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
|State|string|True|The state of the human. Refer to [HumanStateEnum](../Enums/HumanStateEnum.md)|
|CanDodge|bool|False|Whether the human can dodge.|
|IsInvincible|bool|False|Whether the human is invincible.|
|InvincibleTimeLeft|float|False|The time left for invincibility.|
|IsCarried|bool|True|If the human is carried.|
|Grounded|bool|True|If the human is on the ground.|
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
|Target|[Object](../objects/Object.md)|False|The target currently focused by this character. Returns null if no target is set.|
|TargetPosition|[Vector3](../Collections/Vector3.md)|False|The target position of the (AI) human.|
|TargetVelocity|[Vector3](../Collections/Vector3.md)|True|The target velocity of the (AI) human.|
|IsWalking|bool|False|Whether the AI controller should walk instead of run. Defaults to false (run).|
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
<pre class="language-typescript"><code class="lang-typescript">function MountMapObject(mapObject: <a data-footnote-ref href="#user-content-fn-24">MapObject</a>, positionOffset: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationOffset: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, canMountedAttack: bool = False)</code></pre>
> Mounts the human on a map object.
> 
> **Parameters**:
> - `mapObject`: The map object to mount on.
> - `positionOffset`: The position offset from the mount point.
> - `rotationOffset`: The rotation offset from the mount point.
> - `canMountedAttack`: If true, allows the human to attack while mounted (default: false).
> 
<pre class="language-typescript"><code class="lang-typescript">function MountTransform(transform: <a data-footnote-ref href="#user-content-fn-30">Transform</a>, positionOffset: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationOffset: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, canMountedAttack: bool = False)</code></pre>
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
<pre class="language-typescript"><code class="lang-typescript">function MoveTo(position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, range: float)</code></pre>
> Causes the (AI) human to move towards a position and stopping when within specified range.
> 
> **Parameters**:
> - `position`: The target position to move towards.
> - `range`: The stopping range from the target position.
> 
<pre class="language-typescript"><code class="lang-typescript">function MoveToTarget(target: <a data-footnote-ref href="#user-content-fn-122">Object</a>, range: float)</code></pre>
> Causes the (AI) human to move towards a target and stopping when within specified range.
> 
> **Parameters**:
> - `target`: The target to move towards.
> - `range`: The stopping range from the target.
> 
<pre class="language-typescript"><code class="lang-typescript">function Idle()</code></pre>
> Causes the (AI) human to idle.
> 
<pre class="language-typescript"><code class="lang-typescript">function HasAIState(name: string) -> bool</code></pre>
> Determine whether an AIState exists for the (AI) human.
> 
> **Parameters**:
> - `name`: The name of the AI state.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetAIState(name: string, classInstance: UserClassInstance = null)</code></pre>
> Set the custom AI states for the (AI) human.
> 
> **Parameters**:
> - `name`: The name of the AI state.
> - `classInstance`: The class instance for the AI state.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetAIState() -> string</code></pre>
> Get the name of the AI state of the (AI) human.
> 
<pre class="language-typescript"><code class="lang-typescript">function SwitchAIState(name: string)</code></pre>
> Switch the AI state of the (AI) human.
> 
> **Parameters**:
> - `name`: The name of the AI state to switch to.
> 
<pre class="language-typescript"><code class="lang-typescript">function ResetCallback(callback: string, method: function = null)</code></pre>
> Reset the callbacks for the (AI) human. Optional: OnIdle, PreAction, PostAction, MoveToCallback.
> 
> **Parameters**:
> - `callback`: The callback name to reset.
> - `method`: The method to set as the callback.
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
> Causes the (AI) human to attack.
> 
> **Parameters**:
> - `attackOn`: True to start attacking, false to stop.
> 
<pre class="language-typescript"><code class="lang-typescript">function FindNearestEnemy()</code></pre>
> Causes the (AI) human to find the nearest enemy.
> 
<pre class="language-typescript"><code class="lang-typescript">function Navigation()</code></pre>
> Correct the direction of the (AI) human for moving to the target.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetParticleEffect(effectName: string, enabled: bool)</code></pre>
> Enables or disables a particle effect.
> 
> **Parameters**:
> - `effectName`: Name of the effect. Refer to [HumanParticleEffectEnum](../Enums/HumanParticleEffectEnum.md)
> - `enabled`: True to enable, false to disable.
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
