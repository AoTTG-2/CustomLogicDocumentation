# Game
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|IsEnding|bool|False|Is the game ending?|
|EndTimeLeft|float|False|Time left until the game ends|
|Titans|[List](../objects/list.md)|False|List of all titans|
|AITitans|[List](../objects/list.md)|False|List of all AI titans|
|PlayerTitans|[List](../objects/list.md)|False|List of all player titans|
|Shifters|[List](../objects/list.md)|False|List of all shifters|
|AIShifters|[List](../objects/list.md)|False|List of all AI shifters|
|PlayerShifters|[List](../objects/list.md)|False|List of all player shifters|
|Humans|[List](../objects/list.md)|False|List of all humans|
|AIHumans|[List](../objects/list.md)|False|List of all AI humans|
|PlayerHumans|[List](../objects/list.md)|False|List of all player humans|
|Loadouts|[List](../objects/list.md)|False|List of all loadouts|
|DefaultShowKillScore|bool|False|Is the kill score shown by default?|
|DefaultHideKillScore|bool|False|Is the kill feed shown by default?|
|DefaultAddKillScore|bool|False|Is the kill score added by default?|
|ShowScoreboardLoadout|bool|False|Is the loadout shown in the scoreboard?|
|ShowScoreboardStatus|bool|False|Is the status shown in the scoreboard?|
|ForcedCharacterType|[String](../static/string.md)|False|Forced character type|
|ForcedLoadout|[String](../static/string.md)|False|Forced loadout|
## Methods
|Function|Returns|Description|
|---|---|---|
|Debug(message : Object)|none|Print a debug statement to the console|
|Print(message : Object)|none|Print a message to the chat|
|PrintAll(message : Object)|none|Print a message to all players|
|GetGeneralSetting(settingName : [String](../static/string.md))|Object|Get a general setting|
|GetTitanSetting(settingName : [String](../static/string.md))|Object|Get a titan setting|
|GetMiscSetting(settingName : [String](../static/string.md))|Object|Get a misc setting|
|End(delay : float)|none|End the game|
|FindCharacterByViewID(viewID : int)|[Character](../objects/character.md)|Find a character by view ID|
|SpawnTitan(type : [String](../static/string.md))|[Titan](../objects/titan.md)|Spawn a titan|
|SpawnTitanAt(type : [String](../static/string.md), position : [Vector3](../static/vector3.md), rotationY : float = 0)|[Titan](../objects/titan.md)|Spawn a titan at a position|
|SpawnTitans(type : [String](../static/string.md), count : int)|[List](../objects/list.md)|Spawn titans|
|SpawnTitansAsync(type : [String](../static/string.md), count : int)|none|Spawn titans asynchronously|
|SpawnTitansAt(type : [String](../static/string.md), count : int, position : [Vector3](../static/vector3.md), rotationY : float = 0)|[List](../objects/list.md)|Spawn titans at a position|
|SpawnTitansAtAsync(type : [String](../static/string.md), count : int, position : [Vector3](../static/vector3.md), rotationY : float = 0)|none|Spawn titans at a position asynchronously|
|SpawnShifter(type : [String](../static/string.md))|[Shifter](../objects/shifter.md)|Spawn a shifter|
|SpawnShifterAt(type : [String](../static/string.md), position : [Vector3](../static/vector3.md), rotationY : float = 0)|[Shifter](../objects/shifter.md)|Spawn a shifter at a position|
|SpawnProjectile(parameters : Object[])|none|Spawn a projectile|
|SpawnProjectileWithOwner(parameters : Object[])|none|Spawn a projectile with an owner|
|SpawnEffect(parameters : Object[])|none|Spawn an effect|
|SpawnPlayer(player : [Player](../objects/player.md), force : bool)|none|Spawn a player|
|SpawnPlayerAll(force : bool)|none|Spawn a player for all players|
|SpawnPlayerAt(player : [Player](../objects/player.md), force : bool, position : [Vector3](../static/vector3.md), rotationY : float = 0)|none|Spawn a player at a position|
|SpawnPlayerAtAll(force : bool, position : [Vector3](../static/vector3.md), rotationY : float = 0)|none|Spawn a player at a position for all players|
|SetPlaylist(playlist : [String](../static/string.md))|none|Set the music playlist|
|SetSong(song : [String](../static/string.md))|none|Set the music song|
|DrawRay(start : [Vector3](../static/vector3.md), dir : [Vector3](../static/vector3.md), color : [Color](../static/color.md), duration : float)|none|Draw a ray|
|ShowKillScore(damage : int)|none|Show the kill score|
|ShowKillFeed(killer : [String](../static/string.md), victim : [String](../static/string.md), score : int, weapon : [String](../static/string.md))|none|Show the kill feed|
|ShowKillFeedAll(killer : [String](../static/string.md), victim : [String](../static/string.md), score : int, weapon : [String](../static/string.md))|none|Show the kill feed for all players|
