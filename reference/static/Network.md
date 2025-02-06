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
|SendMessage(player : [Player](../objects/Player.md), message : [String](../static/String.md))|none|Send a message to a player|
|SendMessageAll(message : [String](../static/String.md))|none|Send a message to all players|
|SendMessageOthers(message : [String](../static/String.md))|none|Send a message to all players except the sender|
|GetTimestampDifference(timestamp1 : double, timestamp2 : double)|double|Get the difference between two photon timestamps|
|KickPlayer(target : Object, reason : [String](../static/String.md) = .)|none|Kick the given player by id or player reference.|
