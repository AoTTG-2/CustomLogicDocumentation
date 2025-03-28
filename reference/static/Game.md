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
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Debug</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">message</mark>)
Print a debug statement to the console
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Print</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">message</mark>)
Print a message to the chat
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">PrintAll</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">message</mark>)
Print a message to all players
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">GetGeneralSetting</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">settingName</mark>)
Get a general setting
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">GetTitanSetting</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">settingName</mark>)
Get a titan setting
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">GetMiscSetting</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">settingName</mark>)
Get a misc setting
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">End</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">delay</mark>)
End the game
#### <mark style="color:#509cd4;">[Character](../objects/Character.md)</mark> <mark style="color:#dcdcaa;">FindCharacterByViewID</mark>(<mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">viewID</mark>)
Find a character by view ID
#### <mark style="color:#509cd4;">[Titan](../objects/Titan.md)</mark> <mark style="color:#dcdcaa;">SpawnTitan</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">type</mark>)
Spawn a titan
#### <mark style="color:#509cd4;">[Titan](../objects/Titan.md)</mark> <mark style="color:#dcdcaa;">SpawnTitanAt</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">type</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">rotationY</mark> = <mark style="color:#509cd4;">0</mark>)
Spawn a titan at a position
#### <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#dcdcaa;">SpawnTitans</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">type</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">count</mark>)
Spawn titans
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SpawnTitansAsync</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">type</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">count</mark>)
Spawn titans asynchronously
#### <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#dcdcaa;">SpawnTitansAt</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">type</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">count</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">rotationY</mark> = <mark style="color:#509cd4;">0</mark>)
Spawn titans at a position
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SpawnTitansAtAsync</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">type</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">count</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">rotationY</mark> = <mark style="color:#509cd4;">0</mark>)
Spawn titans at a position asynchronously
#### <mark style="color:#509cd4;">[Shifter](../objects/Shifter.md)</mark> <mark style="color:#dcdcaa;">SpawnShifter</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">type</mark>)
Spawn a shifter
#### <mark style="color:#509cd4;">[Shifter](../objects/Shifter.md)</mark> <mark style="color:#dcdcaa;">SpawnShifterAt</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">type</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">rotationY</mark> = <mark style="color:#509cd4;">0</mark>)
Spawn a shifter at a position
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SpawnProjectile</mark>(<mark style="color:#509cd4;">Object[]</mark> <mark style="color:#9cdcfe;">parameters</mark>)
Spawn a projectile
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SpawnProjectileWithOwner</mark>(<mark style="color:#509cd4;">Object[]</mark> <mark style="color:#9cdcfe;">parameters</mark>)
Spawn a projectile with an owner
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SpawnEffect</mark>(<mark style="color:#509cd4;">Object[]</mark> <mark style="color:#9cdcfe;">parameters</mark>)
Spawn an effect
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SpawnPlayer</mark>(<mark style="color:#509cd4;">[Player](../objects/Player.md)</mark> <mark style="color:#9cdcfe;">player</mark>, <mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">force</mark>)
Spawn a player
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SpawnPlayerAll</mark>(<mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">force</mark>)
Spawn a player for all players
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SpawnPlayerAt</mark>(<mark style="color:#509cd4;">[Player](../objects/Player.md)</mark> <mark style="color:#9cdcfe;">player</mark>, <mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">force</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">rotationY</mark> = <mark style="color:#509cd4;">0</mark>)
Spawn a player at a position
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SpawnPlayerAtAll</mark>(<mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">force</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">rotationY</mark> = <mark style="color:#509cd4;">0</mark>)
Spawn a player at a position for all players
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetPlaylist</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">playlist</mark>)
Set the music playlist
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetSong</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">song</mark>)
Set the music song
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">DrawRay</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">start</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">dir</mark>, <mark style="color:#509cd4;">[Color](../objects/Color.md)</mark> <mark style="color:#9cdcfe;">color</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">duration</mark>)
Draw a ray
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ShowKillScore</mark>(<mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">damage</mark>)
Show the kill score
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ShowKillFeed</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">killer</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">victim</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">score</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">weapon</mark>)
Show the kill feed
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ShowKillFeedAll</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">killer</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">victim</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">score</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">weapon</mark>)
Show the kill feed for all players

---

