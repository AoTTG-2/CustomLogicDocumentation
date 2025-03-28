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
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SendMessage</mark>(<mark style="color:Blue;">[Player](../objects/Player.md)</mark> <mark style="color:Yellow;">player</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">message</mark>)
Send a message to a player
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SendMessageAll</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">message</mark>)
Send a message to all players
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SendMessageOthers</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">message</mark>)
Send a message to all players except the sender
#### <mark style="color:Blue;">double</mark> <mark style="color:Yellow;">GetTimestampDifference</mark>(<mark style="color:Blue;">double</mark> <mark style="color:Yellow;">timestamp1</mark>, <mark style="color:Blue;">double</mark> <mark style="color:Yellow;">timestamp2</mark>)
Get the difference between two photon timestamps
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">KickPlayer</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">target</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">reason</mark> = <mark style="color:Blue;">.</mark>)
Kick the given player by id or player reference.

---

