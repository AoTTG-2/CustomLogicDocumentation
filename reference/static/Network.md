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
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SendMessage</mark>(<mark style="color:#509cd4;">[Player](../objects/Player.md)</mark> <mark style="color:#9cdcfe;">player</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">message</mark>)
Send a message to a player
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SendMessageAll</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">message</mark>)
Send a message to all players
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SendMessageOthers</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">message</mark>)
Send a message to all players except the sender
#### <mark style="color:#509cd4;">double</mark> <mark style="color:#dcdcaa;">GetTimestampDifference</mark>(<mark style="color:#509cd4;">double</mark> <mark style="color:#9cdcfe;">timestamp1</mark>, <mark style="color:#509cd4;">double</mark> <mark style="color:#9cdcfe;">timestamp2</mark>)
Get the difference between two photon timestamps
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">KickPlayer</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">reason</mark> = <mark style="color:#509cd4;">.</mark>)
Kick the given player by id or player reference.

---

