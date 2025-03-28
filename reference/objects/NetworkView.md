# NetworkView
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Owner|[Player](../objects/Player.md)|False|The network view's owner.|
## Methods
#### <span style="color:blue;">void</span> <span style="color:yellow;">Transfer</span>(<span style="color:blue;">[Player](../objects/Player.md)</span> player)
> Owner only. Transfer ownership of this NetworkView to another player.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SendMessage</span>(<span style="color:blue;">[Player](../objects/Player.md)</span> target, <span style="color:blue;">[String](../static/String.md)</span> msg)
> Send a message to a target player. This will be received in any of the MapObject attached components through the OnNetworkMessage callback.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SendMessageAll</span>(<span style="color:blue;">[String](../static/String.md)</span> msg)
> Send a message to all players including myself.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SendMessageOthers</span>(<span style="color:blue;">[String](../static/String.md)</span> msg)
> Send a message to players excluding myself.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SendStream</span>(<span style="color:blue;">Object</span> obj)
> Send an object to the network sync stream.             This represents sending data from the object owner to all non-owner observers,             and should only be called in the SendNetworkStream callback in the attached component.             It only works with some object types: primitives and Vector3.
#### <span style="color:blue;">Object</span> <span style="color:yellow;">ReceiveStream</span>()
> Receive an object through the network sync stream.             This represents receiving data from the object owner as a non-owner observer,             and should only be called in the OnNetworkStream callback.

---

