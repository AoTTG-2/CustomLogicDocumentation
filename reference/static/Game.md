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
|Function|Returns|Description|
|---|---|---|
|Debug(message : Object)|none|Print a debug statement to the console|
|Print(message : Object)|none|Print a message to the chat|
|PrintAll(message : Object)|none|Print a message to all players|
|GetGeneralSetting(settingName : [String](../static/String.md))|Object|Get a general setting|
|GetTitanSetting(settingName : [String](../static/String.md))|Object|Get a titan setting|
|GetMiscSetting(settingName : [String](../static/String.md))|Object|Get a misc setting|
|End(delay : float)|none|End the game|
|FindCharacterByViewID(viewID : int)|[Character](../objects/Character.md)|Find a character by view ID|
|SpawnTitan(type : [String](../static/String.md))|[Titan](../objects/Titan.md)|Spawn a titan|
|SpawnTitanAt(<br/>type : [String](../static/String.md),<br/>position : [Vector3](../objects/Vector3.md),<br/>rotationY : float = 0<br/>)|[Titan](../objects/Titan.md)|Spawn a titan at a position|
|SpawnTitans(<br/>type : [String](../static/String.md),<br/>count : int<br/>)|[List](../objects/List.md)|Spawn titans|
|SpawnTitansAsync(<br/>type : [String](../static/String.md),<br/>count : int<br/>)|none|Spawn titans asynchronously|
|SpawnTitansAt(<br/>type : [String](../static/String.md),<br/>count : int,<br/>position : [Vector3](../objects/Vector3.md),<br/>rotationY : float = 0<br/>)|[List](../objects/List.md)|Spawn titans at a position|
|SpawnTitansAtAsync(<br/>type : [String](../static/String.md),<br/>count : int,<br/>position : [Vector3](../objects/Vector3.md),<br/>rotationY : float = 0<br/>)|none|Spawn titans at a position asynchronously|
|SpawnShifter(type : [String](../static/String.md))|[Shifter](../objects/Shifter.md)|Spawn a shifter|
|SpawnShifterAt(<br/>type : [String](../static/String.md),<br/>position : [Vector3](../objects/Vector3.md),<br/>rotationY : float = 0<br/>)|[Shifter](../objects/Shifter.md)|Spawn a shifter at a position|
|SpawnProjectile(parameters : Object[])|none|Spawn a projectile|
|SpawnProjectileWithOwner(parameters : Object[])|none|Spawn a projectile with an owner|
|SpawnEffect(parameters : Object[])|none|Spawn an effect|
|SpawnPlayer(<br/>player : [Player](../objects/Player.md),<br/>force : bool<br/>)|none|Spawn a player|
|SpawnPlayerAll(force : bool)|none|Spawn a player for all players|
|SpawnPlayerAt(<br/>player : [Player](../objects/Player.md),<br/>force : bool,<br/>position : [Vector3](../objects/Vector3.md),<br/>rotationY : float = 0<br/>)|none|Spawn a player at a position|
|SpawnPlayerAtAll(<br/>force : bool,<br/>position : [Vector3](../objects/Vector3.md),<br/>rotationY : float = 0<br/>)|none|Spawn a player at a position for all players|
|SetPlaylist(playlist : [String](../static/String.md))|none|Set the music playlist|
|SetSong(song : [String](../static/String.md))|none|Set the music song|
|DrawRay(<br/>start : [Vector3](../objects/Vector3.md),<br/>dir : [Vector3](../objects/Vector3.md),<br/>color : [Color](../objects/Color.md),<br/>duration : float<br/>)|none|Draw a ray|
|ShowKillScore(damage : int)|none|Show the kill score|
|ShowKillFeed(<br/>killer : [String](../static/String.md),<br/>victim : [String](../static/String.md),<br/>score : int,<br/>weapon : [String](../static/String.md)<br/>)|none|Show the kill feed|
|ShowKillFeedAll(<br/>killer : [String](../static/String.md),<br/>victim : [String](../static/String.md),<br/>score : int,<br/>weapon : [String](../static/String.md)<br/>)|none|Show the kill feed for all players|
