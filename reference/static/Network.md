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
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SendMessage</span>(<span style="color:#509cd4">[Player](../objects/Player.md)</span> <span style="color:#9cdcfe">player</span>, <span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">message</span>)
Send a message to a player
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SendMessageAll</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">message</span>)
Send a message to all players
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SendMessageOthers</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">message</span>)
Send a message to all players except the sender
#### <span style="color:#509cd4">double</span> <span style="color:#dcdcaa">GetTimestampDifference</span>(<span style="color:#509cd4">double</span> <span style="color:#9cdcfe">timestamp1</span>, <span style="color:#509cd4">double</span> <span style="color:#9cdcfe">timestamp2</span>)
Get the difference between two photon timestamps
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">KickPlayer</span>(<span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">target</span>, <span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">reason</span> = <span style="color:#509cd4">.</span>)
Kick the given player by id or player reference.

---

