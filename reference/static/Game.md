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
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Debug</span>(<span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">message</span>)
Print a debug statement to the console
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Print</span>(<span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">message</span>)
Print a message to the chat
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">PrintAll</span>(<span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">message</span>)
Print a message to all players
#### <span style="color:#509cd4">Object</span> <span style="color:#dcdcaa">GetGeneralSetting</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">settingName</span>)
Get a general setting
#### <span style="color:#509cd4">Object</span> <span style="color:#dcdcaa">GetTitanSetting</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">settingName</span>)
Get a titan setting
#### <span style="color:#509cd4">Object</span> <span style="color:#dcdcaa">GetMiscSetting</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">settingName</span>)
Get a misc setting
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">End</span>(<span style="color:#509cd4">float</span> <span style="color:#9cdcfe">delay</span>)
End the game
#### <span style="color:#509cd4">[Character](../objects/Character.md)</span> <span style="color:#dcdcaa">FindCharacterByViewID</span>(<span style="color:#509cd4">int</span> <span style="color:#9cdcfe">viewID</span>)
Find a character by view ID
#### <span style="color:#509cd4">[Titan](../objects/Titan.md)</span> <span style="color:#dcdcaa">SpawnTitan</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">type</span>)
Spawn a titan
#### <span style="color:#509cd4">[Titan](../objects/Titan.md)</span> <span style="color:#dcdcaa">SpawnTitanAt</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">type</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">position</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">rotationY</span> = <span style="color:#509cd4">0</span>)
Spawn a titan at a position
#### <span style="color:#509cd4">[List](../objects/List.md)</span> <span style="color:#dcdcaa">SpawnTitans</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">type</span>, <span style="color:#509cd4">int</span> <span style="color:#9cdcfe">count</span>)
Spawn titans
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SpawnTitansAsync</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">type</span>, <span style="color:#509cd4">int</span> <span style="color:#9cdcfe">count</span>)
Spawn titans asynchronously
#### <span style="color:#509cd4">[List](../objects/List.md)</span> <span style="color:#dcdcaa">SpawnTitansAt</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">type</span>, <span style="color:#509cd4">int</span> <span style="color:#9cdcfe">count</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">position</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">rotationY</span> = <span style="color:#509cd4">0</span>)
Spawn titans at a position
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SpawnTitansAtAsync</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">type</span>, <span style="color:#509cd4">int</span> <span style="color:#9cdcfe">count</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">position</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">rotationY</span> = <span style="color:#509cd4">0</span>)
Spawn titans at a position asynchronously
#### <span style="color:#509cd4">[Shifter](../objects/Shifter.md)</span> <span style="color:#dcdcaa">SpawnShifter</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">type</span>)
Spawn a shifter
#### <span style="color:#509cd4">[Shifter](../objects/Shifter.md)</span> <span style="color:#dcdcaa">SpawnShifterAt</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">type</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">position</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">rotationY</span> = <span style="color:#509cd4">0</span>)
Spawn a shifter at a position
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SpawnProjectile</span>(<span style="color:#509cd4">Object[]</span> <span style="color:#9cdcfe">parameters</span>)
Spawn a projectile
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SpawnProjectileWithOwner</span>(<span style="color:#509cd4">Object[]</span> <span style="color:#9cdcfe">parameters</span>)
Spawn a projectile with an owner
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SpawnEffect</span>(<span style="color:#509cd4">Object[]</span> <span style="color:#9cdcfe">parameters</span>)
Spawn an effect
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SpawnPlayer</span>(<span style="color:#509cd4">[Player](../objects/Player.md)</span> <span style="color:#9cdcfe">player</span>, <span style="color:#509cd4">bool</span> <span style="color:#9cdcfe">force</span>)
Spawn a player
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SpawnPlayerAll</span>(<span style="color:#509cd4">bool</span> <span style="color:#9cdcfe">force</span>)
Spawn a player for all players
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SpawnPlayerAt</span>(<span style="color:#509cd4">[Player](../objects/Player.md)</span> <span style="color:#9cdcfe">player</span>, <span style="color:#509cd4">bool</span> <span style="color:#9cdcfe">force</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">position</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">rotationY</span> = <span style="color:#509cd4">0</span>)
Spawn a player at a position
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SpawnPlayerAtAll</span>(<span style="color:#509cd4">bool</span> <span style="color:#9cdcfe">force</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">position</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">rotationY</span> = <span style="color:#509cd4">0</span>)
Spawn a player at a position for all players
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SetPlaylist</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">playlist</span>)
Set the music playlist
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SetSong</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">song</span>)
Set the music song
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">DrawRay</span>(<span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">start</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">dir</span>, <span style="color:#509cd4">[Color](../objects/Color.md)</span> <span style="color:#9cdcfe">color</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">duration</span>)
Draw a ray
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">ShowKillScore</span>(<span style="color:#509cd4">int</span> <span style="color:#9cdcfe">damage</span>)
Show the kill score
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">ShowKillFeed</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">killer</span>, <span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">victim</span>, <span style="color:#509cd4">int</span> <span style="color:#9cdcfe">score</span>, <span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">weapon</span>)
Show the kill feed
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">ShowKillFeedAll</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">killer</span>, <span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">victim</span>, <span style="color:#509cd4">int</span> <span style="color:#9cdcfe">score</span>, <span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">weapon</span>)
Show the kill feed for all players

---

