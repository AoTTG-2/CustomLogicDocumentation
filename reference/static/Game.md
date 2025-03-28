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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Debug</mark>(<mark style="color:blue;">Object</mark> message)
> Print a debug statement to the console

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Print</mark>(<mark style="color:blue;">Object</mark> message)
> Print a message to the chat

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">PrintAll</mark>(<mark style="color:blue;">Object</mark> message)
> Print a message to all players

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">GetGeneralSetting</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> settingName)
> Get a general setting

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">GetTitanSetting</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> settingName)
> Get a titan setting

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">GetMiscSetting</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> settingName)
> Get a misc setting

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">End</mark>(<mark style="color:blue;">float</mark> delay)
> End the game

#### <mark style="color:blue;">[Character](../objects/Character.md)</mark> <mark style="color:yellow;">FindCharacterByViewID</mark>(<mark style="color:blue;">int</mark> viewID)
> Find a character by view ID

#### <mark style="color:blue;">[Titan](../objects/Titan.md)</mark> <mark style="color:yellow;">SpawnTitan</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> type)
> Spawn a titan

#### <mark style="color:blue;">[Titan](../objects/Titan.md)</mark> <mark style="color:yellow;">SpawnTitanAt</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> type, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> position, <mark style="color:blue;">float</mark> rotationY = <mark style="color:blue;">0</mark>)
> Spawn a titan at a position

#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">SpawnTitans</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> type, <mark style="color:blue;">int</mark> count)
> Spawn titans

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SpawnTitansAsync</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> type, <mark style="color:blue;">int</mark> count)
> Spawn titans asynchronously

#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">SpawnTitansAt</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> type, <mark style="color:blue;">int</mark> count, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> position, <mark style="color:blue;">float</mark> rotationY = <mark style="color:blue;">0</mark>)
> Spawn titans at a position

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SpawnTitansAtAsync</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> type, <mark style="color:blue;">int</mark> count, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> position, <mark style="color:blue;">float</mark> rotationY = <mark style="color:blue;">0</mark>)
> Spawn titans at a position asynchronously

#### <mark style="color:blue;">[Shifter](../objects/Shifter.md)</mark> <mark style="color:yellow;">SpawnShifter</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> type)
> Spawn a shifter

#### <mark style="color:blue;">[Shifter](../objects/Shifter.md)</mark> <mark style="color:yellow;">SpawnShifterAt</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> type, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> position, <mark style="color:blue;">float</mark> rotationY = <mark style="color:blue;">0</mark>)
> Spawn a shifter at a position

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SpawnProjectile</mark>(<mark style="color:blue;">Object[]</mark> parameters)
> Spawn a projectile

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SpawnProjectileWithOwner</mark>(<mark style="color:blue;">Object[]</mark> parameters)
> Spawn a projectile with an owner

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SpawnEffect</mark>(<mark style="color:blue;">Object[]</mark> parameters)
> Spawn an effect

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SpawnPlayer</mark>(<mark style="color:blue;">[Player](../objects/Player.md)</mark> player, <mark style="color:blue;">bool</mark> force)
> Spawn a player

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SpawnPlayerAll</mark>(<mark style="color:blue;">bool</mark> force)
> Spawn a player for all players

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SpawnPlayerAt</mark>(<mark style="color:blue;">[Player](../objects/Player.md)</mark> player, <mark style="color:blue;">bool</mark> force, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> position, <mark style="color:blue;">float</mark> rotationY = <mark style="color:blue;">0</mark>)
> Spawn a player at a position

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SpawnPlayerAtAll</mark>(<mark style="color:blue;">bool</mark> force, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> position, <mark style="color:blue;">float</mark> rotationY = <mark style="color:blue;">0</mark>)
> Spawn a player at a position for all players

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetPlaylist</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> playlist)
> Set the music playlist

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetSong</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> song)
> Set the music song

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">DrawRay</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> start, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> dir, <mark style="color:blue;">[Color](../objects/Color.md)</mark> color, <mark style="color:blue;">float</mark> duration)
> Draw a ray

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ShowKillScore</mark>(<mark style="color:blue;">int</mark> damage)
> Show the kill score

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ShowKillFeed</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> killer, <mark style="color:blue;">[String](../static/String.md)</mark> victim, <mark style="color:blue;">int</mark> score, <mark style="color:blue;">[String](../static/String.md)</mark> weapon)
> Show the kill feed

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ShowKillFeedAll</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> killer, <mark style="color:blue;">[String](../static/String.md)</mark> victim, <mark style="color:blue;">int</mark> score, <mark style="color:blue;">[String](../static/String.md)</mark> weapon)
> Show the kill feed for all players


---

