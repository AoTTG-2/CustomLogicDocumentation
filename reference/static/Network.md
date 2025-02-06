# Network
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|IsMasterClient|bool|False|Is the player the master client|
|Players|[List](../objects/List.md)|False|The list of players in the room|
|MasterClient|[Player](../objects/Player.md)|False|The master client|
|MyPlayer|[Player](../objects/Player.md)|False|The local player|
|NetworkTime|double|False|The network time|
|Ping|int|False|The local player's ping|
## Methods
|Function|Returns|Description|
|---|---|---|
|SendMessage(<br/>player : [Player](../objects/Player.md),<br/>message : [String](../static/String.md)<br/>)|none|Send a message to a player|
|SendMessageAll(message : [String](../static/String.md))|none|Send a message to all players|
|SendMessageOthers(message : [String](../static/String.md))|none|Send a message to all players except the sender|
|GetTimestampDifference(<br/>timestamp1 : double,<br/>timestamp2 : double<br/>)|double|Get the difference between two photon timestamps|
|KickPlayer(<br/>target : Object,<br/>reason : [String](../static/String.md) = .<br/>)|none|Kick the given player by id or player reference.|
