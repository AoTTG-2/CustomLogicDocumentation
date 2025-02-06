# Game
Inherits from object
## Fields
|<div style="width:30%">Field</div>|<div style="width:10%">Type</div>|<div style="width:10%">Readonly</div>|<div style="width:50%">Description</div>|
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
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
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
|SpawnTitanAt(type : [String](../static/String.md),
position : [Vector3](../objects/Vector3.md),
rotationY : float = 0)|[Titan](../objects/Titan.md)|Spawn a titan at a position|
|SpawnTitans(type : [String](../static/String.md),
count : int)|[List](../objects/List.md)|Spawn titans|
|SpawnTitansAsync(type : [String](../static/String.md),
count : int)|none|Spawn titans asynchronously|
|SpawnTitansAt(type : [String](../static/String.md),
count : int,
position : [Vector3](../objects/Vector3.md),
rotationY : float = 0)|[List](../objects/List.md)|Spawn titans at a position|
|SpawnTitansAtAsync(type : [String](../static/String.md),
count : int,
position : [Vector3](../objects/Vector3.md),
rotationY : float = 0)|none|Spawn titans at a position asynchronously|
|SpawnShifter(type : [String](../static/String.md))|[Shifter](../objects/Shifter.md)|Spawn a shifter|
|SpawnShifterAt(type : [String](../static/String.md),
position : [Vector3](../objects/Vector3.md),
rotationY : float = 0)|[Shifter](../objects/Shifter.md)|Spawn a shifter at a position|
|SpawnProjectile(parameters : Object[])|none|Spawn a projectile|
|SpawnProjectileWithOwner(parameters : Object[])|none|Spawn a projectile with an owner|
|SpawnEffect(parameters : Object[])|none|Spawn an effect|
|SpawnPlayer(player : [Player](../objects/Player.md),
force : bool)|none|Spawn a player|
|SpawnPlayerAll(force : bool)|none|Spawn a player for all players|
|SpawnPlayerAt(player : [Player](../objects/Player.md),
force : bool,
position : [Vector3](../objects/Vector3.md),
rotationY : float = 0)|none|Spawn a player at a position|
|SpawnPlayerAtAll(force : bool,
position : [Vector3](../objects/Vector3.md),
rotationY : float = 0)|none|Spawn a player at a position for all players|
|SetPlaylist(playlist : [String](../static/String.md))|none|Set the music playlist|
|SetSong(song : [String](../static/String.md))|none|Set the music song|
|DrawRay(start : [Vector3](../objects/Vector3.md),
dir : [Vector3](../objects/Vector3.md),
color : [Color](../objects/Color.md),
duration : float)|none|Draw a ray|
|ShowKillScore(damage : int)|none|Show the kill score|
|ShowKillFeed(killer : [String](../static/String.md),
victim : [String](../static/String.md),
score : int,
weapon : [String](../static/String.md))|none|Show the kill feed|
|ShowKillFeedAll(killer : [String](../static/String.md),
victim : [String](../static/String.md),
score : int,
weapon : [String](../static/String.md))|none|Show the kill feed for all players|
