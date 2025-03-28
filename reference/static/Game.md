# Game
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|IsEnding|bool|False|Is the game ending?|
|EndTimeLeft|float|False|Time left until the game ends|
|Titans|[List](../objects/List.md)|False|List of all titans|
|AITitans|[List](../objects/List.md)|False|List of all AI titans|
|PlayerTitans|[List](../objects/List.md)|False|List of all player titans|
|Shifters|[List](../objects/List.md)|False|List of all shifters|
|AIShifters|[List](../objects/List.md)|False|List of all AI shifters|
|PlayerShifters|[List](../objects/List.md)|False|List of all player shifters|
|Humans|[List](../objects/List.md)|False|List of all humans|
|AIHumans|[List](../objects/List.md)|False|List of all AI humans|
|PlayerHumans|[List](../objects/List.md)|False|List of all player humans|
|Loadouts|[List](../objects/List.md)|False|List of all loadouts|
|DefaultShowKillScore|bool|False|Is the kill score shown by default?|
|DefaultHideKillScore|bool|False|Is the kill feed shown by default?|
|DefaultAddKillScore|bool|False|Is the kill score added by default?|
|ShowScoreboardLoadout|bool|False|Is the loadout shown in the scoreboard?|
|ShowScoreboardStatus|bool|False|Is the status shown in the scoreboard?|
|ForcedCharacterType|[String](../static/String.md)|False|Forced character type|
|ForcedLoadout|[String](../static/String.md)|False|Forced loadout|
## Methods
#### <span style="color:blue;">void</span> <span style="color:yellow;">Debug</span>(<span style="color:blue;">Object</span> message)
> Print a debug statement to the console
#### <span style="color:blue;">void</span> <span style="color:yellow;">Print</span>(<span style="color:blue;">Object</span> message)
> Print a message to the chat
#### <span style="color:blue;">void</span> <span style="color:yellow;">PrintAll</span>(<span style="color:blue;">Object</span> message)
> Print a message to all players
#### <span style="color:blue;">Object</span> <span style="color:yellow;">GetGeneralSetting</span>(<span style="color:blue;">[String](../static/String.md)</span> settingName)
> Get a general setting
#### <span style="color:blue;">Object</span> <span style="color:yellow;">GetTitanSetting</span>(<span style="color:blue;">[String](../static/String.md)</span> settingName)
> Get a titan setting
#### <span style="color:blue;">Object</span> <span style="color:yellow;">GetMiscSetting</span>(<span style="color:blue;">[String](../static/String.md)</span> settingName)
> Get a misc setting
#### <span style="color:blue;">void</span> <span style="color:yellow;">End</span>(<span style="color:blue;">float</span> delay)
> End the game
#### <span style="color:blue;">[Character](../objects/Character.md)</span> <span style="color:yellow;">FindCharacterByViewID</span>(<span style="color:blue;">int</span> viewID)
> Find a character by view ID
#### <span style="color:blue;">[Titan](../objects/Titan.md)</span> <span style="color:yellow;">SpawnTitan</span>(<span style="color:blue;">[String](../static/String.md)</span> type)
> Spawn a titan
#### <span style="color:blue;">[Titan](../objects/Titan.md)</span> <span style="color:yellow;">SpawnTitanAt</span>(<span style="color:blue;">[String](../static/String.md)</span> type, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position, <span style="color:blue;">float</span> rotationY = <span style="color:blue;">0</span>)
> Spawn a titan at a position
#### <span style="color:blue;">[List](../objects/List.md)</span> <span style="color:yellow;">SpawnTitans</span>(<span style="color:blue;">[String](../static/String.md)</span> type, <span style="color:blue;">int</span> count)
> Spawn titans
#### <span style="color:blue;">void</span> <span style="color:yellow;">SpawnTitansAsync</span>(<span style="color:blue;">[String](../static/String.md)</span> type, <span style="color:blue;">int</span> count)
> Spawn titans asynchronously
#### <span style="color:blue;">[List](../objects/List.md)</span> <span style="color:yellow;">SpawnTitansAt</span>(<span style="color:blue;">[String](../static/String.md)</span> type, <span style="color:blue;">int</span> count, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position, <span style="color:blue;">float</span> rotationY = <span style="color:blue;">0</span>)
> Spawn titans at a position
#### <span style="color:blue;">void</span> <span style="color:yellow;">SpawnTitansAtAsync</span>(<span style="color:blue;">[String](../static/String.md)</span> type, <span style="color:blue;">int</span> count, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position, <span style="color:blue;">float</span> rotationY = <span style="color:blue;">0</span>)
> Spawn titans at a position asynchronously
#### <span style="color:blue;">[Shifter](../objects/Shifter.md)</span> <span style="color:yellow;">SpawnShifter</span>(<span style="color:blue;">[String](../static/String.md)</span> type)
> Spawn a shifter
#### <span style="color:blue;">[Shifter](../objects/Shifter.md)</span> <span style="color:yellow;">SpawnShifterAt</span>(<span style="color:blue;">[String](../static/String.md)</span> type, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position, <span style="color:blue;">float</span> rotationY = <span style="color:blue;">0</span>)
> Spawn a shifter at a position
#### <span style="color:blue;">void</span> <span style="color:yellow;">SpawnProjectile</span>(<span style="color:blue;">Object[]</span> parameters)
> Spawn a projectile
#### <span style="color:blue;">void</span> <span style="color:yellow;">SpawnProjectileWithOwner</span>(<span style="color:blue;">Object[]</span> parameters)
> Spawn a projectile with an owner
#### <span style="color:blue;">void</span> <span style="color:yellow;">SpawnEffect</span>(<span style="color:blue;">Object[]</span> parameters)
> Spawn an effect
#### <span style="color:blue;">void</span> <span style="color:yellow;">SpawnPlayer</span>(<span style="color:blue;">[Player](../objects/Player.md)</span> player, <span style="color:blue;">bool</span> force)
> Spawn a player
#### <span style="color:blue;">void</span> <span style="color:yellow;">SpawnPlayerAll</span>(<span style="color:blue;">bool</span> force)
> Spawn a player for all players
#### <span style="color:blue;">void</span> <span style="color:yellow;">SpawnPlayerAt</span>(<span style="color:blue;">[Player](../objects/Player.md)</span> player, <span style="color:blue;">bool</span> force, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position, <span style="color:blue;">float</span> rotationY = <span style="color:blue;">0</span>)
> Spawn a player at a position
#### <span style="color:blue;">void</span> <span style="color:yellow;">SpawnPlayerAtAll</span>(<span style="color:blue;">bool</span> force, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position, <span style="color:blue;">float</span> rotationY = <span style="color:blue;">0</span>)
> Spawn a player at a position for all players
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetPlaylist</span>(<span style="color:blue;">[String](../static/String.md)</span> playlist)
> Set the music playlist
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetSong</span>(<span style="color:blue;">[String](../static/String.md)</span> song)
> Set the music song
#### <span style="color:blue;">void</span> <span style="color:yellow;">DrawRay</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> start, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> dir, <span style="color:blue;">[Color](../objects/Color.md)</span> color, <span style="color:blue;">float</span> duration)
> Draw a ray
#### <span style="color:blue;">void</span> <span style="color:yellow;">ShowKillScore</span>(<span style="color:blue;">int</span> damage)
> Show the kill score
#### <span style="color:blue;">void</span> <span style="color:yellow;">ShowKillFeed</span>(<span style="color:blue;">[String](../static/String.md)</span> killer, <span style="color:blue;">[String](../static/String.md)</span> victim, <span style="color:blue;">int</span> score, <span style="color:blue;">[String](../static/String.md)</span> weapon)
> Show the kill feed
#### <span style="color:blue;">void</span> <span style="color:yellow;">ShowKillFeedAll</span>(<span style="color:blue;">[String](../static/String.md)</span> killer, <span style="color:blue;">[String](../static/String.md)</span> victim, <span style="color:blue;">int</span> score, <span style="color:blue;">[String](../static/String.md)</span> weapon)
> Show the kill feed for all players

---

