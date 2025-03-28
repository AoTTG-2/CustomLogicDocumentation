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
#### void <span style="color":#dcdcaa>Debug<span>(Object <span style="color":#9cdcfe>message<span>)
Print a debug statement to the console
#### void <span style="color":#dcdcaa>Print<span>(Object <span style="color":#9cdcfe>message<span>)
Print a message to the chat
#### void <span style="color":#dcdcaa>PrintAll<span>(Object <span style="color":#9cdcfe>message<span>)
Print a message to all players
#### Object <span style="color":#dcdcaa>GetGeneralSetting<span>([String](../static/String.md) <span style="color":#9cdcfe>settingName<span>)
Get a general setting
#### Object <span style="color":#dcdcaa>GetTitanSetting<span>([String](../static/String.md) <span style="color":#9cdcfe>settingName<span>)
Get a titan setting
#### Object <span style="color":#dcdcaa>GetMiscSetting<span>([String](../static/String.md) <span style="color":#9cdcfe>settingName<span>)
Get a misc setting
#### void <span style="color":#dcdcaa>End<span>(float <span style="color":#9cdcfe>delay<span>)
End the game
#### [Character](../objects/Character.md) <span style="color":#dcdcaa>FindCharacterByViewID<span>(int <span style="color":#9cdcfe>viewID<span>)
Find a character by view ID
#### [Titan](../objects/Titan.md) <span style="color":#dcdcaa>SpawnTitan<span>([String](../static/String.md) <span style="color":#9cdcfe>type<span>)
Spawn a titan
#### [Titan](../objects/Titan.md) <span style="color":#dcdcaa>SpawnTitanAt<span>([String](../static/String.md) <span style="color":#9cdcfe>type<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>, float <span style="color":#9cdcfe>rotationY<span> = 0)
Spawn a titan at a position
#### [List](../objects/List.md) <span style="color":#dcdcaa>SpawnTitans<span>([String](../static/String.md) <span style="color":#9cdcfe>type<span>, int <span style="color":#9cdcfe>count<span>)
Spawn titans
#### void <span style="color":#dcdcaa>SpawnTitansAsync<span>([String](../static/String.md) <span style="color":#9cdcfe>type<span>, int <span style="color":#9cdcfe>count<span>)
Spawn titans asynchronously
#### [List](../objects/List.md) <span style="color":#dcdcaa>SpawnTitansAt<span>([String](../static/String.md) <span style="color":#9cdcfe>type<span>, int <span style="color":#9cdcfe>count<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>, float <span style="color":#9cdcfe>rotationY<span> = 0)
Spawn titans at a position
#### void <span style="color":#dcdcaa>SpawnTitansAtAsync<span>([String](../static/String.md) <span style="color":#9cdcfe>type<span>, int <span style="color":#9cdcfe>count<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>, float <span style="color":#9cdcfe>rotationY<span> = 0)
Spawn titans at a position asynchronously
#### [Shifter](../objects/Shifter.md) <span style="color":#dcdcaa>SpawnShifter<span>([String](../static/String.md) <span style="color":#9cdcfe>type<span>)
Spawn a shifter
#### [Shifter](../objects/Shifter.md) <span style="color":#dcdcaa>SpawnShifterAt<span>([String](../static/String.md) <span style="color":#9cdcfe>type<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>, float <span style="color":#9cdcfe>rotationY<span> = 0)
Spawn a shifter at a position
#### void <span style="color":#dcdcaa>SpawnProjectile<span>(Object[] <span style="color":#9cdcfe>parameters<span>)
Spawn a projectile
#### void <span style="color":#dcdcaa>SpawnProjectileWithOwner<span>(Object[] <span style="color":#9cdcfe>parameters<span>)
Spawn a projectile with an owner
#### void <span style="color":#dcdcaa>SpawnEffect<span>(Object[] <span style="color":#9cdcfe>parameters<span>)
Spawn an effect
#### void <span style="color":#dcdcaa>SpawnPlayer<span>([Player](../objects/Player.md) <span style="color":#9cdcfe>player<span>, bool <span style="color":#9cdcfe>force<span>)
Spawn a player
#### void <span style="color":#dcdcaa>SpawnPlayerAll<span>(bool <span style="color":#9cdcfe>force<span>)
Spawn a player for all players
#### void <span style="color":#dcdcaa>SpawnPlayerAt<span>([Player](../objects/Player.md) <span style="color":#9cdcfe>player<span>, bool <span style="color":#9cdcfe>force<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>, float <span style="color":#9cdcfe>rotationY<span> = 0)
Spawn a player at a position
#### void <span style="color":#dcdcaa>SpawnPlayerAtAll<span>(bool <span style="color":#9cdcfe>force<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>, float <span style="color":#9cdcfe>rotationY<span> = 0)
Spawn a player at a position for all players
#### void <span style="color":#dcdcaa>SetPlaylist<span>([String](../static/String.md) <span style="color":#9cdcfe>playlist<span>)
Set the music playlist
#### void <span style="color":#dcdcaa>SetSong<span>([String](../static/String.md) <span style="color":#9cdcfe>song<span>)
Set the music song
#### void <span style="color":#dcdcaa>DrawRay<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>start<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>dir<span>, [Color](../objects/Color.md) <span style="color":#9cdcfe>color<span>, float <span style="color":#9cdcfe>duration<span>)
Draw a ray
#### void <span style="color":#dcdcaa>ShowKillScore<span>(int <span style="color":#9cdcfe>damage<span>)
Show the kill score
#### void <span style="color":#dcdcaa>ShowKillFeed<span>([String](../static/String.md) <span style="color":#9cdcfe>killer<span>, [String](../static/String.md) <span style="color":#9cdcfe>victim<span>, int <span style="color":#9cdcfe>score<span>, [String](../static/String.md) <span style="color":#9cdcfe>weapon<span>)
Show the kill feed
#### void <span style="color":#dcdcaa>ShowKillFeedAll<span>([String](../static/String.md) <span style="color":#9cdcfe>killer<span>, [String](../static/String.md) <span style="color":#9cdcfe>victim<span>, int <span style="color":#9cdcfe>score<span>, [String](../static/String.md) <span style="color":#9cdcfe>weapon<span>)
Show the kill feed for all players

---

