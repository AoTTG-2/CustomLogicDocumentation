# NetworkView
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Owner|[Player](../objects/Player.md)|False|The network view's owner.|
## Methods
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Transfer</mark>(<mark style="color:#509cd4;">[Player](../objects/Player.md)</mark> <mark style="color:#9cdcfe;">player</mark>)
Owner only. Transfer ownership of this NetworkView to another player.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SendMessage</mark>(<mark style="color:#509cd4;">[Player](../objects/Player.md)</mark> <mark style="color:#9cdcfe;">target</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">msg</mark>)
Send a message to a target player. This will be received in any of the MapObject attached components through the OnNetworkMessage callback.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SendMessageAll</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">msg</mark>)
Send a message to all players including myself.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SendMessageOthers</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">msg</mark>)
Send a message to players excluding myself.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SendStream</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">obj</mark>)
Send an object to the network sync stream.             This represents sending data from the object owner to all non-owner observers,             and should only be called in the SendNetworkStream callback in the attached component.             It only works with some object types: primitives and Vector3.
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">ReceiveStream</mark>()
Receive an object through the network sync stream.             This represents receiving data from the object owner as a non-owner observer,             and should only be called in the OnNetworkStream callback.

---

