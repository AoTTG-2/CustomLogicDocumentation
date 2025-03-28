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
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Debug</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">message</mark>)
Print a debug statement to the console
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Print</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">message</mark>)
Print a message to the chat
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">PrintAll</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">message</mark>)
Print a message to all players
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">GetGeneralSetting</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">settingName</mark>)
Get a general setting
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">GetTitanSetting</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">settingName</mark>)
Get a titan setting
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">GetMiscSetting</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">settingName</mark>)
Get a misc setting
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">End</mark>(<mark style="color:Blue;">float</mark> <mark style="color:Yellow;">delay</mark>)
End the game
#### <mark style="color:Blue;">[Character](../objects/Character.md)</mark> <mark style="color:Yellow;">FindCharacterByViewID</mark>(<mark style="color:Blue;">int</mark> <mark style="color:Yellow;">viewID</mark>)
Find a character by view ID
#### <mark style="color:Blue;">[Titan](../objects/Titan.md)</mark> <mark style="color:Yellow;">SpawnTitan</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">type</mark>)
Spawn a titan
#### <mark style="color:Blue;">[Titan](../objects/Titan.md)</mark> <mark style="color:Yellow;">SpawnTitanAt</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">type</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">position</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">rotationY</mark> = <mark style="color:Blue;">0</mark>)
Spawn a titan at a position
#### <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">SpawnTitans</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">type</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">count</mark>)
Spawn titans
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SpawnTitansAsync</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">type</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">count</mark>)
Spawn titans asynchronously
#### <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">SpawnTitansAt</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">type</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">count</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">position</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">rotationY</mark> = <mark style="color:Blue;">0</mark>)
Spawn titans at a position
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SpawnTitansAtAsync</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">type</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">count</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">position</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">rotationY</mark> = <mark style="color:Blue;">0</mark>)
Spawn titans at a position asynchronously
#### <mark style="color:Blue;">[Shifter](../objects/Shifter.md)</mark> <mark style="color:Yellow;">SpawnShifter</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">type</mark>)
Spawn a shifter
#### <mark style="color:Blue;">[Shifter](../objects/Shifter.md)</mark> <mark style="color:Yellow;">SpawnShifterAt</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">type</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">position</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">rotationY</mark> = <mark style="color:Blue;">0</mark>)
Spawn a shifter at a position
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SpawnProjectile</mark>(<mark style="color:Blue;">Object[]</mark> <mark style="color:Yellow;">parameters</mark>)
Spawn a projectile
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SpawnProjectileWithOwner</mark>(<mark style="color:Blue;">Object[]</mark> <mark style="color:Yellow;">parameters</mark>)
Spawn a projectile with an owner
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SpawnEffect</mark>(<mark style="color:Blue;">Object[]</mark> <mark style="color:Yellow;">parameters</mark>)
Spawn an effect
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SpawnPlayer</mark>(<mark style="color:Blue;">[Player](../objects/Player.md)</mark> <mark style="color:Yellow;">player</mark>, <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">force</mark>)
Spawn a player
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SpawnPlayerAll</mark>(<mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">force</mark>)
Spawn a player for all players
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SpawnPlayerAt</mark>(<mark style="color:Blue;">[Player](../objects/Player.md)</mark> <mark style="color:Yellow;">player</mark>, <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">force</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">position</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">rotationY</mark> = <mark style="color:Blue;">0</mark>)
Spawn a player at a position
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SpawnPlayerAtAll</mark>(<mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">force</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">position</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">rotationY</mark> = <mark style="color:Blue;">0</mark>)
Spawn a player at a position for all players
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetPlaylist</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">playlist</mark>)
Set the music playlist
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetSong</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">song</mark>)
Set the music song
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">DrawRay</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">start</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">dir</mark>, <mark style="color:Blue;">[Color](../objects/Color.md)</mark> <mark style="color:Yellow;">color</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">duration</mark>)
Draw a ray
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">ShowKillScore</mark>(<mark style="color:Blue;">int</mark> <mark style="color:Yellow;">damage</mark>)
Show the kill score
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">ShowKillFeed</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">killer</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">victim</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">score</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">weapon</mark>)
Show the kill feed
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">ShowKillFeedAll</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">killer</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">victim</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">score</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">weapon</mark>)
Show the kill feed for all players

---

