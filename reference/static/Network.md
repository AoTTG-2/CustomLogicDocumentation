# Network
Inherits from object
## Fields
|<div style="width:30%">Field</div>|<div style="width:5%">Type</div>|<div style="width:5%">Readonly</div>|<div style="width:60%">Description</div>|
|---|---|---|---|
|IsMasterClient|bool|False|Is the player the master client|
|Players|[List](../objects/List.md)|False|The list of players in the room|
|MasterClient|[Player](../objects/Player.md)|False|The master client|
|MyPlayer|[Player](../objects/Player.md)|False|The local player|
|NetworkTime|double|False|The network time|
|Ping|int|False|The local player's ping|
## Methods
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|SendMessage(player : [Player](../objects/Player.md),<br/>message : [String](../static/String.md))|none|Send a message to a player|
|SendMessageAll(message : [String](../static/String.md))|none|Send a message to all players|
|SendMessageOthers(message : [String](../static/String.md))|none|Send a message to all players except the sender|
|GetTimestampDifference(timestamp1 : double,<br/>timestamp2 : double)|double|Get the difference between two photon timestamps|
|KickPlayer(target : Object,<br/>reason : [String](../static/String.md) = .)|none|Kick the given player by id or player reference.|
