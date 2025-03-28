# NetworkView
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Owner|[Player](../objects/Player.md)|False|The network view's owner.|
## Methods
#### void <span style="color":#dcdcaa>Transfer<span>([Player](../objects/Player.md) <span style="color":#9cdcfe>player<span>)
Owner only. Transfer ownership of this NetworkView to another player.
#### void <span style="color":#dcdcaa>SendMessage<span>([Player](../objects/Player.md) <span style="color":#9cdcfe>target<span>, [String](../static/String.md) <span style="color":#9cdcfe>msg<span>)
Send a message to a target player. This will be received in any of the MapObject attached components through the OnNetworkMessage callback.
#### void <span style="color":#dcdcaa>SendMessageAll<span>([String](../static/String.md) <span style="color":#9cdcfe>msg<span>)
Send a message to all players including myself.
#### void <span style="color":#dcdcaa>SendMessageOthers<span>([String](../static/String.md) <span style="color":#9cdcfe>msg<span>)
Send a message to players excluding myself.
#### void <span style="color":#dcdcaa>SendStream<span>(Object <span style="color":#9cdcfe>obj<span>)
Send an object to the network sync stream.             This represents sending data from the object owner to all non-owner observers,             and should only be called in the SendNetworkStream callback in the attached component.             It only works with some object types: primitives and Vector3.
#### Object <span style="color":#dcdcaa>ReceiveStream<span>()
Receive an object through the network sync stream.             This represents receiving data from the object owner as a non-owner observer,             and should only be called in the OnNetworkStream callback.

---

