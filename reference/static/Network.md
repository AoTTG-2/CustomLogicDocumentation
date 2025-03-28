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
#### <span style="color:blue;">void</span> <span style="color:yellow;">SendMessage</span>(<span style="color:blue;">[Player](../objects/Player.md)</span> player, <span style="color:blue;">[String](../static/String.md)</span> message)
> Send a message to a player
#### <span style="color:blue;">void</span> <span style="color:yellow;">SendMessageAll</span>(<span style="color:blue;">[String](../static/String.md)</span> message)
> Send a message to all players
#### <span style="color:blue;">void</span> <span style="color:yellow;">SendMessageOthers</span>(<span style="color:blue;">[String](../static/String.md)</span> message)
> Send a message to all players except the sender
#### <span style="color:blue;">double</span> <span style="color:yellow;">GetTimestampDifference</span>(<span style="color:blue;">double</span> timestamp1, <span style="color:blue;">double</span> timestamp2)
> Get the difference between two photon timestamps
#### <span style="color:blue;">void</span> <span style="color:yellow;">KickPlayer</span>(<span style="color:blue;">Object</span> target, <span style="color:blue;">[String](../static/String.md)</span> reason = <span style="color:blue;">.</span>)
> Kick the given player by id or player reference.

---

