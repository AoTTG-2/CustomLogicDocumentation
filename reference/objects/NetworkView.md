# NetworkView
Inherits from object
## Fields
|<div style="width:30%">Field</div>|<div style="width:10%">Type</div>|<div style="width:10%">Readonly</div>|<div style="width:50%">Description</div>|
|---|---|---|---|
|Owner|[Player](../objects/Player.md)|False|The network view's owner.|
## Methods
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|Transfer(player : [Player](../objects/Player.md))|none|Owner only. Transfer ownership of this NetworkView to another player.|
|SendMessage(target : [Player](../objects/Player.md),<br/>msg : [String](../static/String.md))|none|Send a message to a target player. This will be received in any of the MapObject attached components through the OnNetworkMessage callback.|
|SendMessageAll(msg : [String](../static/String.md))|none|Send a message to all players including myself.|
|SendMessageOthers(msg : [String](../static/String.md))|none|Send a message to players excluding myself.|
|SendStream(obj : Object)|none|Send an object to the network sync stream.             This represents sending data from the object owner to all non-owner observers,             and should only be called in the SendNetworkStream callback in the attached component.             It only works with some object types: primitives and Vector3.|
|ReceiveStream()|Object|Receive an object through the network sync stream.             This represents receiving data from the object owner as a non-owner observer,             and should only be called in the OnNetworkStream callback.|
