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
#### void <span style="color":#dcdcaa>SendMessage<span>([Player](../objects/Player.md) <span style="color":#9cdcfe>player<span>, [String](../static/String.md) <span style="color":#9cdcfe>message<span>)
Send a message to a player
#### void <span style="color":#dcdcaa>SendMessageAll<span>([String](../static/String.md) <span style="color":#9cdcfe>message<span>)
Send a message to all players
#### void <span style="color":#dcdcaa>SendMessageOthers<span>([String](../static/String.md) <span style="color":#9cdcfe>message<span>)
Send a message to all players except the sender
#### double <span style="color":#dcdcaa>GetTimestampDifference<span>(double <span style="color":#9cdcfe>timestamp1<span>, double <span style="color":#9cdcfe>timestamp2<span>)
Get the difference between two photon timestamps
#### void <span style="color":#dcdcaa>KickPlayer<span>(Object <span style="color":#9cdcfe>target<span>, [String](../static/String.md) <span style="color":#9cdcfe>reason<span> = .)
Kick the given player by id or player reference.

---

