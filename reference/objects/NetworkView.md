# NetworkView
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Owner|[Player](../objects/Player.md)|False|The network view's owner.|
## Methods
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Transfer</mark>(<mark style="color:Blue;">[Player](../objects/Player.md)</mark> <mark style="color:Yellow;">player</mark>)
Owner only. Transfer ownership of this NetworkView to another player.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SendMessage</mark>(<mark style="color:Blue;">[Player](../objects/Player.md)</mark> <mark style="color:Yellow;">target</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">msg</mark>)
Send a message to a target player. This will be received in any of the MapObject attached components through the OnNetworkMessage callback.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SendMessageAll</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">msg</mark>)
Send a message to all players including myself.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SendMessageOthers</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">msg</mark>)
Send a message to players excluding myself.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SendStream</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">obj</mark>)
Send an object to the network sync stream.             This represents sending data from the object owner to all non-owner observers,             and should only be called in the SendNetworkStream callback in the attached component.             It only works with some object types: primitives and Vector3.
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">ReceiveStream</mark>()
Receive an object through the network sync stream.             This represents receiving data from the object owner as a non-owner observer,             and should only be called in the OnNetworkStream callback.

---

