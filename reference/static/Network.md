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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SendMessage</mark>(<mark style="color:blue;">[Player](../objects/Player.md)</mark> <mark style="color:yellow;">player</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">message</mark>)
Send a message to a player
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SendMessageAll</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">message</mark>)
Send a message to all players
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SendMessageOthers</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">message</mark>)
Send a message to all players except the sender
#### <mark style="color:blue;">double</mark> <mark style="color:yellow;">GetTimestampDifference</mark>(<mark style="color:blue;">double</mark> <mark style="color:yellow;">timestamp1</mark>, <mark style="color:blue;">double</mark> <mark style="color:yellow;">timestamp2</mark>)
Get the difference between two photon timestamps
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">KickPlayer</mark>(<mark style="color:blue;">Object</mark> <mark style="color:yellow;">target</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">reason</mark> = <mark style="color:blue;">.</mark>)
Kick the given player by id or player reference.

---

