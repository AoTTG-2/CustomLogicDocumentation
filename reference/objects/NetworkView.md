# NetworkView
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Owner|[Player](../objects/Player.md)|False|The network view's owner.|
## Methods
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Transfer</span>(<span style="color:#509cd4;">[Player](../objects/Player.md)</span> <span style="color:#9cdcfe;">player</span>)
Owner only. Transfer ownership of this NetworkView to another player.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SendMessage</span>(<span style="color:#509cd4;">[Player](../objects/Player.md)</span> <span style="color:#9cdcfe;">target</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">msg</span>)
Send a message to a target player. This will be received in any of the MapObject attached components through the OnNetworkMessage callback.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SendMessageAll</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">msg</span>)
Send a message to all players including myself.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SendMessageOthers</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">msg</span>)
Send a message to players excluding myself.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SendStream</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">obj</span>)
Send an object to the network sync stream.             This represents sending data from the object owner to all non-owner observers,             and should only be called in the SendNetworkStream callback in the attached component.             It only works with some object types: primitives and Vector3.
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">ReceiveStream</span>()
Receive an object through the network sync stream.             This represents receiving data from the object owner as a non-owner observer,             and should only be called in the OnNetworkStream callback.

---

