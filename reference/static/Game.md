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
|Debug(<i>message</i> : Object)|none|Print a debug statement to the console|
|Print(<i>message</i> : Object)|none|Print a message to the chat|
|PrintAll(<i>message</i> : Object)|none|Print a message to all players|
|GetGeneralSetting(<i>settingName</i> : [String](../static/String.md))|Object|Get a general setting|
|GetTitanSetting(<i>settingName</i> : [String](../static/String.md))|Object|Get a titan setting|
|GetMiscSetting(<i>settingName</i> : [String](../static/String.md))|Object|Get a misc setting|
|End(<i>delay</i> : float)|none|End the game|
|FindCharacterByViewID(<i>viewID</i> : int)|[Character](../objects/Character.md)|Find a character by view ID|
|SpawnTitan(<i>type</i> : [String](../static/String.md))|[Titan](../objects/Titan.md)|Spawn a titan|
|SpawnTitanAt(<br/><i>type</i> : [String](../static/String.md),<br/><i>position</i> : [Vector3](../objects/Vector3.md),<br/><i>rotationY</i> : float = 0<br/>)|[Titan](../objects/Titan.md)|Spawn a titan at a position|
|SpawnTitans(<br/><i>type</i> : [String](../static/String.md),<br/><i>count</i> : int<br/>)|[List](../objects/List.md)|Spawn titans|
|SpawnTitansAsync(<br/><i>type</i> : [String](../static/String.md),<br/><i>count</i> : int<br/>)|none|Spawn titans asynchronously|
|SpawnTitansAt(<br/><i>type</i> : [String](../static/String.md),<br/><i>count</i> : int,<br/><i>position</i> : [Vector3](../objects/Vector3.md),<br/><i>rotationY</i> : float = 0<br/>)|[List](../objects/List.md)|Spawn titans at a position|
|SpawnTitansAtAsync(<br/><i>type</i> : [String](../static/String.md),<br/><i>count</i> : int,<br/><i>position</i> : [Vector3](../objects/Vector3.md),<br/><i>rotationY</i> : float = 0<br/>)|none|Spawn titans at a position asynchronously|
|SpawnShifter(<i>type</i> : [String](../static/String.md))|[Shifter](../objects/Shifter.md)|Spawn a shifter|
|SpawnShifterAt(<br/><i>type</i> : [String](../static/String.md),<br/><i>position</i> : [Vector3](../objects/Vector3.md),<br/><i>rotationY</i> : float = 0<br/>)|[Shifter](../objects/Shifter.md)|Spawn a shifter at a position|
|SpawnProjectile(<i>parameters</i> : Object[])|none|Spawn a projectile|
|SpawnProjectileWithOwner(<i>parameters</i> : Object[])|none|Spawn a projectile with an owner|
|SpawnEffect(<i>parameters</i> : Object[])|none|Spawn an effect|
|SpawnPlayer(<br/><i>player</i> : [Player](../objects/Player.md),<br/><i>force</i> : bool<br/>)|none|Spawn a player|
|SpawnPlayerAll(<i>force</i> : bool)|none|Spawn a player for all players|
|SpawnPlayerAt(<br/><i>player</i> : [Player](../objects/Player.md),<br/><i>force</i> : bool,<br/><i>position</i> : [Vector3](../objects/Vector3.md),<br/><i>rotationY</i> : float = 0<br/>)|none|Spawn a player at a position|
|SpawnPlayerAtAll(<br/><i>force</i> : bool,<br/><i>position</i> : [Vector3](../objects/Vector3.md),<br/><i>rotationY</i> : float = 0<br/>)|none|Spawn a player at a position for all players|
|SetPlaylist(<i>playlist</i> : [String](../static/String.md))|none|Set the music playlist|
|SetSong(<i>song</i> : [String](../static/String.md))|none|Set the music song|
|DrawRay(<br/><i>start</i> : [Vector3](../objects/Vector3.md),<br/><i>dir</i> : [Vector3](../objects/Vector3.md),<br/><i>color</i> : [Color](../objects/Color.md),<br/><i>duration</i> : float<br/>)|none|Draw a ray|
|ShowKillScore(<i>damage</i> : int)|none|Show the kill score|
|ShowKillFeed(<br/><i>killer</i> : [String](../static/String.md),<br/><i>victim</i> : [String](../static/String.md),<br/><i>score</i> : int,<br/><i>weapon</i> : [String](../static/String.md)<br/>)|none|Show the kill feed|
|ShowKillFeedAll(<br/><i>killer</i> : [String](../static/String.md),<br/><i>victim</i> : [String](../static/String.md),<br/><i>score</i> : int,<br/><i>weapon</i> : [String](../static/String.md)<br/>)|none|Show the kill feed for all players|
