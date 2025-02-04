# NetworkView

Inherits from Object. Represents a network view on a map object that has the "networked" flag.

### Fields

<table><thead><tr><th width="175.33333333333331">Field</th><th width="99">Type</th><th width="113">Readonly</th><th>Description</th></tr></thead><tbody><tr><td>Owner</td><td>Player</td><td>true</td><td>The network view's owner.</td></tr></tbody></table>

### Functions

<table><thead><tr><th width="254.33333333333331">Function</th><th width="94">Returns</th><th>Description</th></tr></thead><tbody><tr><td>Transfer(target: Player)</td><td>null</td><td>Owner only. Transfer ownership of this NetworkView to another player.</td></tr><tr><td>SendMessage(target: Player, message: string)</td><td>null</td><td>Send a message to a target player. This will be received in any of the MapObject attached components through the OnNetworkMessage callback.</td></tr><tr><td>SendMessageAll(message: string)</td><td>null</td><td>Send a message to all players including myself.</td></tr><tr><td>SendMessageOthers(message: string)</td><td>null</td><td>Send a message to players excluding myself.</td></tr><tr><td>SendStream(item: Object)</td><td>null</td><td>Send an object to the network sync stream. This represents sending data from the object owner to all non-owner observers, and should only be called in the SendNetworkStream callback in the attached component. It only works with some object types: primitives and Vector3.</td></tr><tr><td>ReceiveStream(item: Object)</td><td>null</td><td>Receive an object through the network sync stream. This represents receiving data from the object owner as a non-owner observer, and should only be called in the OnNetworkStream callback.</td></tr></tbody></table>

