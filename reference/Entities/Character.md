# Character
Inherits from [Object](../objects/Object.md)

Character is the base class that `Human`, `Horse`, `Titan`, and `Shifter` inherit from.
Only character owner can modify properties and call functions unless otherwise specified.

### Remarks
Overloads operators: 
`==`, `__Hash__`
### Example
```csharp
function OnCharacterSpawn(character)
{
    if (character.IsMine)
    {
        # Character is owned (network-wise) by the person running this script.
        # Ex: If user is host, this could either be their actual player character or AI titans/shifters.
    }

    if (character.IsMainCharacter)
    {
        # Character is the main character (the camera-followed player).
    }

    if (character.IsAI)
    {
        # Character is AI and likely controlled via MasterClient.

        if (character.Player.ID == Network.MasterClient.ID)
        {
            # Character is owned by masterclient, if we're not masterclient, we cannot modify props.
        }
    }
}
```
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|CurrentTarget|[Object](../objects/Object.md)|True|(AI) current target, or null.|
|DetectRange|float|False|(AI) character's detection range in world units.|
|State|string|True|Character state name.|
|IsWalking|bool|False|(AI) whether to walk instead of run.|
|AIEnabled|bool|False|(AI) enables automatic behavior.|
|UsePathfinding|bool|False|Whether AI movement uses navmesh paths.|
|Name|string|False|Character's name.|
|Guild|string|False|Character's guild.|
|Player|[Player](../Entities/Player.md)|True|Player who owns this character.|
|IsAI|bool|True|Is this character AI?|
|IsAlive|bool|True|Is this character alive? Value is set to false before despawn.|
|ViewID|int|True|Network view ID of the character.|
|IsMine|bool|True|Is this character mine?|
|IsMainCharacter|bool|True|Character belongs to my player and is the main character (the camera-followed player).|
|Transform|[Transform](../Entities/Transform.md)|True|Unity transform of the character.|
|Position|[Vector3](../Collections/Vector3.md)|False|Position of the character.|
|Rotation|[Vector3](../Collections/Vector3.md)|False|Rotation of the character.|
|QuaternionRotation|[Quaternion](../Collections/Quaternion.md)|False|Quaternion rotation of the character.|
|Velocity|[Vector3](../Collections/Vector3.md)|False|Velocity of the character.|
|Forward|[Vector3](../Collections/Vector3.md)|False|Forward direction of the character.|
|Right|[Vector3](../Collections/Vector3.md)|False|Right direction of the character.|
|Up|[Vector3](../Collections/Vector3.md)|False|Up direction of the character.|
|HasTargetDirection|bool|True|If the character has a target direction it is turning towards.|
|TargetDirection|[Vector3](../Collections/Vector3.md)|False|The character's target direction.|
|Team|string|False|Team character belongs to. Using enum is not mandatory, value can be any string. Refer to [TeamEnum](../Enums/TeamEnum.md)|
|Health|float|False|Character's current health.|
|MaxHealth|float|False|Character's maximum health.|
|CustomDamageEnabled|bool|False|Is custom damage dealing enabled.|
|CustomDamage|int|False|Amount of custom damage to deal per attack.|
|CurrentAnimation|string|True|Character's current playing animation.|
|Grounded|bool|True|Character's grounded status.|
|Rigidbody|[RigidbodyBuiltin](../Component/RigidbodyBuiltin.md)|True|Character's rigidbody component (if available).|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function GetTarget() -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Gets the (AI) character's current target.
> 
> **Returns**: A Character or MapTargetable, or null.
<pre class="language-typescript"><code class="lang-typescript">function SetTarget(target: <a data-footnote-ref href="#user-content-fn-127">Object</a>, focusDuration: float = 0)</code></pre>
> Sets the (AI) character's target.
> 
> **Parameters**:
> - `target`: A Character or MapTargetable, or null to clear.
> - `focusDuration`: Focus time in seconds. 0 uses the default.
> 
<pre class="language-typescript"><code class="lang-typescript">function ClearTarget()</code></pre>
> Clears the combat target of an (AI) character.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetNearestEnemy() -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Finds the nearest enemy or map targetable within DetectRange.
> 
> **Returns**: A Character or MapTargetable, or null.
<pre class="language-typescript"><code class="lang-typescript">function TargetNearestEnemy(focusDuration: float = 0)</code></pre>
> (AI) targets the nearest enemy.
> 
> **Parameters**:
> - `focusDuration`: Focus time in seconds. 0 uses the default.
> 
<pre class="language-typescript"><code class="lang-typescript">function MoveTo(position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, range: float, ignoreEnemies: bool = False)</code></pre>
> Moves the (AI) character to a position.
> 
> **Parameters**:
> - `position`: Target position.
> - `range`: Stopping distance.
> - `ignoreEnemies`: Ignore enemies during movement. Default: false.
> 
<pre class="language-typescript"><code class="lang-typescript">function MoveToTarget(target: <a data-footnote-ref href="#user-content-fn-127">Object</a>, range: float, ignoreEnemies: bool = False)</code></pre>
> Moves the (AI) character within range of a target.
> 
> **Parameters**:
> - `target`: A Character or MapTargetable.
> - `range`: Stopping distance.
> - `ignoreEnemies`: Ignore enemies during movement. Default: false.
> 
<pre class="language-typescript"><code class="lang-typescript">function Idle(time: float = -1)</code></pre>
> Stops the (AI) character's movement and targeting.
> 
> **Parameters**:
> - `time`: Idle time in seconds. Default: 0 for humans, indefinite for titans and shifters.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetDisplayName(name: string, showTag: bool = True)</code></pre>
> Sets the character display name and optionally enables name tag rendering for AI.
Use this for AI spawned characters when you want their name popup to appear.
> 
> **Parameters**:
> - `name`: Display name text.
> - `showTag`: If true, enables AI name popup when the name is non-empty. Default is true.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetKilled(killer: string)</code></pre>
> Kills the character.
> 
> **Parameters**:
> - `killer`: Killer name.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetDamaged(killer: string, damage: int)</code></pre>
> Damages the character.
> 
> **Parameters**:
> - `killer`: Killer name.
> - `damage`: Damage amount.
> 
<pre class="language-typescript"><code class="lang-typescript">function Emote(emote: string)</code></pre>
> Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.
> 
> **Parameters**:
> - `emote`: Name of the emote to play.
> 
<pre class="language-typescript"><code class="lang-typescript">function PlayAnimation(animation: string, fade: float = 0.1)</code></pre>
> Causes the character to play an animation. Available animations can be found here: Human, Titan, Annie, Eren.
Use the right-hand string value for the animation. Note that shifters also have all titan animations.
> 
> **Parameters**:
> - `animation`: Name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> - `fade`: Fade time. If provided, will crossfade the animation by this timestep.
> 
<pre class="language-typescript"><code class="lang-typescript">function PlayAnimationAt(animation: string, t: float, fade: float = 0.1, force: bool = False)</code></pre>
> Causes the character to play an animation at a specific time.
> 
> **Parameters**:
> - `animation`: Name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> - `t`: Time in the animation to start playing.
> - `fade`: Fade time.
> - `force`: Whether to force the animation even if it's already playing.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetAnimationSpeed(animation: string) -> float</code></pre>
> Gets the animation speed of a given animation.
> 
> **Parameters**:
> - `animation`: Name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> 
> **Returns**: 1.0 if the character is not owned by the player or is dead, otherwise the animation speed.
<pre class="language-typescript"><code class="lang-typescript">function SetAnimationSpeed(animation: string, speed: float, synced: bool = True)</code></pre>
> Sets the animation speed of a given animation.
> 
> **Parameters**:
> - `animation`: Name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> - `speed`: The animation speed multiplier.
> - `synced`: Whether to sync the speed across the network.
> 
<pre class="language-typescript"><code class="lang-typescript">function IsPlayingAnimation(animation: string) -> bool</code></pre>
> Returns true if the animation is playing.
> 
> **Parameters**:
> - `animation`: Name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> 
> **Returns**: True if the animation is playing, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function GetAnimationNormalizedTime(animation: string) -> float</code></pre>
> Gets the normalized time of the currently playing animation.
> 
> **Parameters**:
> - `animation`: Name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> 
> **Returns**: The normalized time (0-1) of the animation.
<pre class="language-typescript"><code class="lang-typescript">function ForceAnimation(animation: string, fade: float = 0.1)</code></pre>
> Forces the character to play an animation, even if it's already playing.
Available animations can be found here: Human, Titan, Annie, Eren.
Use the right-hand string value for the animation. Note that shifters also have all titan animations.
> 
> **Parameters**:
> - `animation`: Name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> - `fade`: Fade time. If provided, will crossfade the animation by this timestep.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetAnimationLength(animation: string) -> float</code></pre>
> Gets the length of animation.
> 
> **Parameters**:
> - `animation`: Name of the animation. Refer to [HumanAnimationEnum](../Enums/HumanAnimationEnum.md), [TitanAnimationEnum](../Enums/TitanAnimationEnum.md), [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md), [ErenAnimationEnum](../Enums/ErenAnimationEnum.md), [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md), [DummyAnimationEnum](../Enums/DummyAnimationEnum.md), [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
> 
> **Returns**: The length of the animation in seconds.
<pre class="language-typescript"><code class="lang-typescript">function IsPlayingSound(sound: string) -> bool</code></pre>
> Returns true if the character is playing a sound.
Available sound names can be found here: Humans, Shifters, Titans.
Note that shifters also have all titan sounds.
> 
> **Parameters**:
> - `sound`: Name of the sound. Refer to [HumanSoundEnum](../Enums/HumanSoundEnum.md), [TitanSoundEnum](../Enums/TitanSoundEnum.md), [ShifterSoundEnum](../Enums/ShifterSoundEnum.md)
> 
> **Returns**: True if the sound is playing, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function PlaySound(sound: string, local: bool = False)</code></pre>
> Plays a sound for the character.
Available sound names can be found here: Human, Shifters, Titans.
Note that shifters also have all titan sounds.
> 
> **Parameters**:
> - `sound`: Name of the sound to play. Refer to [HumanSoundEnum](../Enums/HumanSoundEnum.md), [TitanSoundEnum](../Enums/TitanSoundEnum.md), [ShifterSoundEnum](../Enums/ShifterSoundEnum.md)
> - `local`: If true, the sound only plays for the local client and is not networked.
> 
<pre class="language-typescript"><code class="lang-typescript">function StopSound(sound: string)</code></pre>
> Stops a sound for the character.
> 
> **Parameters**:
> - `sound`: Name of the sound to stop. Refer to [HumanSoundEnum](../Enums/HumanSoundEnum.md), [TitanSoundEnum](../Enums/TitanSoundEnum.md), [ShifterSoundEnum](../Enums/ShifterSoundEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function FadeSound(sound: string, volume: float, time: float)</code></pre>
> Fades the sound volume to a specific volume between 0.0 and 1.0 over [time] seconds.
Does not play or stop the sound.
> 
> **Parameters**:
> - `sound`: Name of the sound. Refer to [HumanSoundEnum](../Enums/HumanSoundEnum.md), [TitanSoundEnum](../Enums/TitanSoundEnum.md), [ShifterSoundEnum](../Enums/ShifterSoundEnum.md)
> - `volume`: Target volume (0.0 to 1.0).
> - `time`: Time in seconds to fade over.
> 
<pre class="language-typescript"><code class="lang-typescript">function LookAt(position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>)</code></pre>
> Rotates the character such that it is looking towards a world position.
> 
> **Parameters**:
> - `position`: The world position to look at.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddForce(force: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, mode: int)</code></pre>
> Adds a force to the character with given force vector and optional mode.
> 
> **Parameters**:
> - `force`: Force vector.
> - `mode`: Force mode. Default is Acceleration. Refer to [ForceModeEnum](../Enums/ForceModeEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function Reveal(delay: float)</code></pre>
> Reveal the titan for a set number of seconds.
> 
> **Parameters**:
> - `delay`: Delay in seconds before revealing.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddOutline(color: <a data-footnote-ref href="#user-content-fn-0">Color</a> = null, mode: string = "OutlineAll")</code></pre>
> Adds an outline effect with the given color and mode.
> 
> **Parameters**:
> - `color`: Outline color.
> - `mode`: Outline mode. Default is OutlineAll. Refer to [OutlineModeEnum](../Enums/OutlineModeEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function RemoveOutline()</code></pre>
> Removes the outline effect from the character.
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
