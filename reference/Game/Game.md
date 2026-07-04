# Game
Inherits from [Object](../objects/Object.md)

Game functions such as spawning titans and managing game state.

### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|IsEnding|bool|True|Is the game ending?|
|EndTimeLeft|float|True|Time left until the game ends.|
|Titans|[List](../Collections/List.md)<[Titan](../Entities/Titan.md)>|True|List of all titans.|
|AITitans|[List](../Collections/List.md)<[Titan](../Entities/Titan.md)>|True|List of all AI titans.|
|PlayerTitans|[List](../Collections/List.md)<[Titan](../Entities/Titan.md)>|True|List of all player titans.|
|Shifters|[List](../Collections/List.md)<[Shifter](../Entities/Shifter.md)>|True|List of all shifters.|
|AIShifters|[List](../Collections/List.md)<[Shifter](../Entities/Shifter.md)>|True|List of all AI shifters.|
|PlayerShifters|[List](../Collections/List.md)<[Shifter](../Entities/Shifter.md)>|True|List of all player shifters.|
|Humans|[List](../Collections/List.md)<[Human](../Entities/Human.md)>|True|List of all humans.|
|AIHumans|[List](../Collections/List.md)<[Human](../Entities/Human.md)>|True|List of all AI humans.|
|PlayerHumans|[List](../Collections/List.md)<[Human](../Entities/Human.md)>|True|List of all player humans.|
|Loadouts|[List](../Collections/List.md)<string>|True|List of all loadouts.|
|DefaultShowKillScore|bool|False|Is the kill score shown by default?|
|DefaultHideKillScore|bool|False|Is the kill feed shown by default?|
|DefaultAddKillScore|bool|False|Is the kill score added by default?|
|ShowScoreboardLoadout|bool|False|Is the loadout shown in the scoreboard?|
|ShowScoreboardStatus|bool|False|Is the status shown in the scoreboard?|
|ForcedCharacterType|string|False|Forced character type. Refer to [CharacterTypeEnum](../Enums/CharacterTypeEnum.md)|
|ForcedLoadout|string|False|Forced loadout. Refer to [LoadoutEnum](../Enums/LoadoutEnum.md)|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function SpawnHuman(costume: int, costumeName: string, loadout: string) -> <a data-footnote-ref href="#user-content-fn-23">Human</a></code></pre>
> Spawn an AI human.
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnHumanAt(costume: int, costumeName: string, loadout: string, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationY: float = 0) -> <a data-footnote-ref href="#user-content-fn-23">Human</a></code></pre>
> Spawn an AI human at a position.
> 

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Debug(message: <a data-footnote-ref href="#user-content-fn-122">Object</a>)</code></pre>
> Print a debug statement to the console.
> 
> **Parameters**:
> - `message`: The message to print.
> 
<pre class="language-typescript"><code class="lang-typescript">function Print(message: <a data-footnote-ref href="#user-content-fn-122">Object</a>)</code></pre>
> Print a message to the chat.
> 
> **Parameters**:
> - `message`: The message to print.
> 
<pre class="language-typescript"><code class="lang-typescript">function PrintAll(message: <a data-footnote-ref href="#user-content-fn-122">Object</a>)</code></pre>
> Print a message to all players.
> 
> **Parameters**:
> - `message`: The message to print.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetGeneralSetting(settingName: string) -> <a data-footnote-ref href="#user-content-fn-122">Object</a></code></pre>
> Get a general setting.
> 
> **Parameters**:
> - `settingName`: The name of the setting to get.
> 
> **Returns**: The setting value.
<pre class="language-typescript"><code class="lang-typescript">function GetTitanSetting(settingName: string) -> <a data-footnote-ref href="#user-content-fn-122">Object</a></code></pre>
> Get a titan setting.
> 
> **Parameters**:
> - `settingName`: The name of the setting to get.
> 
> **Returns**: The setting value.
<pre class="language-typescript"><code class="lang-typescript">function GetMiscSetting(settingName: string) -> <a data-footnote-ref href="#user-content-fn-122">Object</a></code></pre>
> Get a misc setting.
> 
> **Parameters**:
> - `settingName`: The name of the setting to get.
> 
> **Returns**: The setting value.
<pre class="language-typescript"><code class="lang-typescript">function SetPreloadGeneralSetting(settingName: string, value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Set a pre-load general setting (applied on next restart).
Only the master client can call this.
> 
> **Parameters**:
> - `settingName`: The general setting name.
> - `value`: The new value.
> 
> **Returns**: True if updated, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function SetPreloadTitanSetting(settingName: string, value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Set a pre-load titan setting (applied on next restart).
Only the master client can call this.
> 
> **Parameters**:
> - `settingName`: The titan setting name.
> - `value`: The new value.
> 
> **Returns**: True if updated, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function SetPreloadMiscSetting(settingName: string, value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Set a pre-load misc setting (applied on next restart).
Only the master client can call this.
> 
> **Parameters**:
> - `settingName`: The misc setting name.
> - `value`: The new value.
> 
> **Returns**: True if updated, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function SetPreloadModeSetting(settingName: string, value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Set a pre-load mode setting (applied on next restart).
Only the master client can call this.
> 
> **Parameters**:
> - `settingName`: The mode setting name.
> - `value`: The new value.
> 
> **Returns**: True if updated, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function SetPreloadMap(mapCategory: string, mapName: string) -> bool</code></pre>
> Set pre-load map selection (applied on next restart).
Only the master client can call this.
> 
> **Parameters**:
> - `mapCategory`: The map category.
> - `mapName`: The map name.
> 
> **Returns**: True if updated, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function SetPreloadGameMode(gameMode: string) -> bool</code></pre>
> Set pre-load game mode selection (applied on next restart).
Only the master client can call this.
> 
> **Parameters**:
> - `gameMode`: The game mode.
> 
> **Returns**: True if updated, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function LoadPreloadPreset(presetName: string) -> bool</code></pre>
> Load pre-load settings from a named preset (applied on next restart).
Only the master client can call this.
> 
> **Parameters**:
> - `presetName`: The preset name.
> 
> **Returns**: True if the preset exists and was loaded, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function RestartWithPreloadSettings() -> bool</code></pre>
> Restart the game so pre-load settings are copied and used for the next round.
Only the master client can call this.
> 
> **Returns**: True if restart was triggered, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function End(delay: float)</code></pre>
> End the game.
> 
> **Parameters**:
> - `delay`: The delay in seconds before ending the game.
> 
<pre class="language-typescript"><code class="lang-typescript">function FindCharacterByViewID(viewID: int) -> <a data-footnote-ref href="#user-content-fn-22">Character</a></code></pre>
> Find a character by view ID.
> 
> **Parameters**:
> - `viewID`: The Photon view ID of the character.
> 
> **Returns**: The character if found, null otherwise.
<pre class="language-typescript"><code class="lang-typescript">function SpawnTitan(type: string) -> <a data-footnote-ref href="#user-content-fn-29">Titan</a></code></pre>
> Spawn a titan.
> 
> **Parameters**:
> - `type`: The type of titan to spawn. Refer to [TitanTypeEnum](../Enums/TitanTypeEnum.md)
> 
> **Returns**: The spawned titan, or null if not master client.
<pre class="language-typescript"><code class="lang-typescript">function SpawnTitanAt(type: string, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationY: float = 0) -> <a data-footnote-ref href="#user-content-fn-29">Titan</a></code></pre>
> Spawn a titan at a position.
> 
> **Parameters**:
> - `type`: The type of titan to spawn. Refer to [TitanTypeEnum](../Enums/TitanTypeEnum.md)
> - `position`: The spawn position.
> - `rotationY`: The Y rotation in degrees (default: 0).
> 
> **Returns**: The spawned titan, or null if not master client.
<pre class="language-typescript"><code class="lang-typescript">function SpawnTitans(type: string, count: int) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-29">Titan</a>></code></pre>
> Spawn titans.
> 
> **Parameters**:
> - `type`: The type of titan to spawn. Refer to [TitanTypeEnum](../Enums/TitanTypeEnum.md)
> - `count`: The number of titans to spawn.
> 
> **Returns**: A list of spawned titans, or null if not master client.
<pre class="language-typescript"><code class="lang-typescript">function SpawnTitansAsync(type: string, count: int)</code></pre>
> Spawn titans asynchronously.
> 
> **Parameters**:
> - `type`: The type of titan to spawn. Refer to [TitanTypeEnum](../Enums/TitanTypeEnum.md)
> - `count`: The number of titans to spawn.
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnTitansAt(type: string, count: int, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationY: float = 0) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-29">Titan</a>></code></pre>
> Spawn titans at a position.
> 
> **Parameters**:
> - `type`: The type of titan to spawn. Refer to [TitanTypeEnum](../Enums/TitanTypeEnum.md)
> - `count`: The number of titans to spawn.
> - `position`: The spawn position.
> - `rotationY`: The Y rotation in degrees (default: 0).
> 
> **Returns**: A list of spawned titans, or null if not master client.
<pre class="language-typescript"><code class="lang-typescript">function SpawnTitansAtAsync(type: string, count: int, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationY: float = 0)</code></pre>
> Spawn titans at a position asynchronously.
> 
> **Parameters**:
> - `type`: The type of titan to spawn. Refer to [TitanTypeEnum](../Enums/TitanTypeEnum.md)
> - `count`: The number of titans to spawn.
> - `position`: The spawn position.
> - `rotationY`: The Y rotation in degrees (default: 0).
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnShifter(type: string) -> <a data-footnote-ref href="#user-content-fn-28">Shifter</a></code></pre>
> Spawn a shifter.
> 
> **Parameters**:
> - `type`: The type of shifter to spawn. Refer to [ShifterTypeEnum](../Enums/ShifterTypeEnum.md)
> 
> **Returns**: The spawned shifter, or null if not master client.
<pre class="language-typescript"><code class="lang-typescript">function SpawnShifterAt(type: string, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationY: float = 0) -> <a data-footnote-ref href="#user-content-fn-28">Shifter</a></code></pre>
> Spawn a shifter at a position.
> 
> **Parameters**:
> - `type`: The type of shifter to spawn. Refer to [ShifterTypeEnum](../Enums/ShifterTypeEnum.md)
> - `position`: The spawn position.
> - `rotationY`: The Y rotation in degrees (default: 0).
> 
> **Returns**: The spawned shifter, or null if not master client.
<pre class="language-typescript"><code class="lang-typescript">function SpawnProjectile(projectileName: string, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotation: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, velocity: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, gravity: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, liveTime: float, team: string, extraParam: <a data-footnote-ref href="#user-content-fn-122">Object</a> = null, extraParam2: <a data-footnote-ref href="#user-content-fn-122">Object</a> = null)</code></pre>
> Spawn a projectile. Note: `extraParam` and `extraParam2` are optional.
They may or may not be used depending on the value of `projectileName`.
> 
> **Parameters**:
> - `projectileName`: Name of the projectile. Refer to [ProjectileNameEnum](../Enums/ProjectileNameEnum.md)
> - `position`: Spawn position.
> - `rotation`: Spawn rotation.
> - `velocity`: Spawn velocity.
> - `gravity`: Spawn gravity.
> - `liveTime`: Live time of the projectile.
> - `team`: The team that the projectile belongs to. Refer to [TeamEnum](../Enums/TeamEnum.md)
> - `extraParam`: Optional. Type depends on projectile: Thunderspear: float (explosion radius), Flare: Color (flare color), Rock1: float (rock size), Others: unused.
> - `extraParam2`: Optional. Type depends on projectile: Thunderspear: Color (projectile color), Others: unused.
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnProjectileWithOwner(projectileName: string, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotation: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, velocity: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, gravity: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, liveTime: float, owner: <a data-footnote-ref href="#user-content-fn-22">Character</a>, extraParam: <a data-footnote-ref href="#user-content-fn-122">Object</a> = null, extraParam2: <a data-footnote-ref href="#user-content-fn-122">Object</a> = null)</code></pre>
> Spawn a projectile with an owner. Note: `extraParam` and `extraParam2` are optional.
They may or may not be used depending on the value of `projectileName`.
> 
> **Parameters**:
> - `projectileName`: Name of the projectile. Refer to [ProjectileNameEnum](../Enums/ProjectileNameEnum.md)
> - `position`: Spawn position.
> - `rotation`: Spawn rotation.
> - `velocity`: Spawn velocity.
> - `gravity`: Spawn gravity.
> - `liveTime`: Live time of the projectile.
> - `owner`: The character that the projectile belongs to.
> - `extraParam`: Optional. Type depends on projectile: Thunderspear: float (explosion radius), Flare: Color (flare color), Rock1: float (rock size), Others: unused.
> - `extraParam2`: Optional. Type depends on projectile: Thunderspear: Color (projectile color), Others: unused.
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnEffect(effectName: string, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotation: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, scale: float, tsExplodeColor: <a data-footnote-ref href="#user-content-fn-0">Color</a> = null, tsKillSound: string = null)</code></pre>
> Spawn an effect.
> 
> **Parameters**:
> - `effectName`: Name of the effect. Refer to [EffectNameEnum](../Enums/EffectNameEnum.md)
> - `position`: Spawn position.
> - `rotation`: Spawn rotation.
> - `scale`: Spawn scale.
> - `tsExplodeColor`: Thunderspear explode color (Only valid when effectName is "ThunderspearExplode").
> - `tsKillSound`: Optional. Thunderspear explode sound (Only valid when effectName is "ThunderspearExplode"). Refer to [TSKillSoundEnum](../Enums/TSKillSoundEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnUnscaledEffect(effectName: string, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotation: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, tsExplodeColor: <a data-footnote-ref href="#user-content-fn-0">Color</a> = null, tsKillSound: string = null)</code></pre>
> Spawn an unscaled effect.
> 
> **Parameters**:
> - `effectName`: Name of the effect. Refer to [EffectNameEnum](../Enums/EffectNameEnum.md)
> - `position`: Spawn position.
> - `rotation`: Spawn rotation.
> - `tsExplodeColor`: Thunderspear explode color (Only valid when effectName is "ThunderspearExplode").
> - `tsKillSound`: Optional. Thunderspear explode sound (Only valid when effectName is "ThunderspearExplode"). Refer to [TSKillSoundEnum](../Enums/TSKillSoundEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnPlayer(player: <a data-footnote-ref href="#user-content-fn-26">Player</a>, force: bool)</code></pre>
> Spawn a player.
> 
> **Parameters**:
> - `player`: The player to spawn.
> - `force`: If true, forces respawn even if the player is already alive.
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnPlayerAll(force: bool)</code></pre>
> Spawn a player for all players.
> 
> **Parameters**:
> - `force`: If true, forces respawn even if players are already alive.
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnPlayerAt(player: <a data-footnote-ref href="#user-content-fn-26">Player</a>, force: bool, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationY: float = 0)</code></pre>
> Spawn a player at a position.
> 
> **Parameters**:
> - `player`: The player to spawn.
> - `force`: If true, forces respawn even if the player is already alive.
> - `position`: The spawn position.
> - `rotationY`: The Y rotation in degrees (default: 0).
> 
<pre class="language-typescript"><code class="lang-typescript">function SpawnPlayerAtAll(force: bool, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationY: float = 0)</code></pre>
> Spawn a player at a position for all players.
> 
> **Parameters**:
> - `force`: If true, forces respawn even if players are already alive.
> - `position`: The spawn position.
> - `rotationY`: The Y rotation in degrees (default: 0).
> 
<pre class="language-typescript"><code class="lang-typescript">function SetPlaylist(playlist: string)</code></pre>
> Set the music playlist.
> 
> **Parameters**:
> - `playlist`: The name of the playlist to set.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetSong(song: string)</code></pre>
> Set the music song.
> 
> **Parameters**:
> - `song`: The name of the song to set.
> 
<pre class="language-typescript"><code class="lang-typescript">function DrawRay(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, dir: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, color: <a data-footnote-ref href="#user-content-fn-0">Color</a>, duration: float)</code></pre>
> Draw a ray.
> 
> **Parameters**:
> - `start`: The start position of the ray.
> - `dir`: The direction vector of the ray.
> - `color`: The color of the ray.
> - `duration`: The duration in seconds to display the ray.
> 
<pre class="language-typescript"><code class="lang-typescript">function ShowKillScore(damage: int)</code></pre>
> Show the kill score.
> 
> **Parameters**:
> - `damage`: The damage value to display.
> 
<pre class="language-typescript"><code class="lang-typescript">function ShowKillFeed(killer: string, victim: string, score: int, weapon: string)</code></pre>
> Show the kill feed.
> 
> **Parameters**:
> - `killer`: The name of the killer.
> - `victim`: The name of the victim.
> - `score`: The score value.
> - `weapon`: The weapon name.
> 
<pre class="language-typescript"><code class="lang-typescript">function ShowKillFeedAll(killer: string, victim: string, score: int, weapon: string)</code></pre>
> Show the kill feed for all players.
> 
> **Parameters**:
> - `killer`: The name of the killer.
> - `victim`: The name of the victim.
> - `score`: The score value.
> - `weapon`: The weapon name.
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
