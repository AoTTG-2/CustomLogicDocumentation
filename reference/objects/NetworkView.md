# NetworkView
Inherits from [Object](../objects/Object.md)

Represents a network view on a map object that has the "networked" flag.
Note1: messages sent from a mapobjects network view are not component scoped, all components will receive the same message.
If you intend for a mapobject to have multiple message sending components, preface the message with the component name to determine scope.

Note2: Rooms and Players have bandwidth limits, exceeding the limits via CL will result in either the player being kicked or the room being shut down.
When possible, use basic message passing for state sync and then run logic locally instead of repeatedly sending state over the network. Also
avoid cases where message sending increases heavily with the number of players in the room.

### Example
```csharp
# The following is for a component scoped object, in general this is bad practice if the component is widely used.
# OnPlayerJoin, every object with this component will send a message to the player that joined, if you use 100 objects with this, 100 messages will be sent.
# Preferred practice for this sort of case is to have a either Main handle the single message pass or have a single ManagerComponent that handles the message pass
# and defers the value to all registered components.
KillCount = 0;

function OnNetworkMessage(player, message, sentServerTime) {
if (player.ID == Network.MasterClient.ID) {
self.KillCount == Convert.ToInt(message);
}
}

function OnCharacterDie(victim, killer, killerName) {
self.KillCount += 1;
}

function OnPlayerJoined(player) {
if (Network.IsMasterClient) {
self.NetworkView.SendMessage(player, Convert.ToString(self.KillCount));
}
}

# Good Practice would be to have a single component that handles the message pass and defers the value to all registered components.
TODO: Bother someone for good practice example - maybe move this into Networking Summary Page.
```
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Owner|[Player](../objects/Player.md)|True|The network view's owner.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Transfer(player: <a data-footnote-ref href="#user-content-fn-Player">Player</a>) -> null</code></pre>
> Owner only. Transfer ownership of this NetworkView to another player.

<pre class="language-typescript"><code class="lang-typescript">function SendMessage(target: <a data-footnote-ref href="#user-content-fn-Player">Player</a>, msg: string) -> null</code></pre>
> Send a message to a target player. This will be received in any of the MapObject attached components through the OnNetworkMessage callback.

<pre class="language-typescript"><code class="lang-typescript">function SendMessageAll(msg: string) -> null</code></pre>
> Send a message to all players including myself.

<pre class="language-typescript"><code class="lang-typescript">function SendMessageOthers(msg: string) -> null</code></pre>
> Send a message to players excluding myself.

<pre class="language-typescript"><code class="lang-typescript">function SendStream(obj: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Send an object to the network sync stream.
This represents sending data from the object owner to all non-owner observers,
and should only be called in the SendNetworkStream callback in the attached component.
It only works with some object types: primitives and Vector3.

<pre class="language-typescript"><code class="lang-typescript">function ReceiveStream() -> <a data-footnote-ref href="#user-content-fn-Object">Object</a></code></pre>
> Receive an object through the network sync stream.
This represents receiving data from the object owner as a non-owner observer,
and should only be called in the OnNetworkStream callback.


[^Camera]: [Camera](../static/Camera.md)
[^Character]: [Character](../objects/Character.md)
[^Collider]: [Collider](../objects/Collider.md)
[^Collision]: [Collision](../objects/Collision.md)
[^Color]: [Color](../objects/Color.md)
[^Convert]: [Convert](../static/Convert.md)
[^Cutscene]: [Cutscene](../static/Cutscene.md)
[^Dict]: [Dict](../objects/Dict.md)
[^Game]: [Game](../static/Game.md)
[^Human]: [Human](../objects/Human.md)
[^Input]: [Input](../static/Input.md)
[^Json]: [Json](../static/Json.md)
[^LineCastHitResult]: [LineCastHitResult](../objects/LineCastHitResult.md)
[^LineRenderer]: [LineRenderer](../objects/LineRenderer.md)
[^List]: [List](../objects/List.md)
[^Map]: [Map](../static/Map.md)
[^MapObject]: [MapObject](../objects/MapObject.md)
[^MapTargetable]: [MapTargetable](../objects/MapTargetable.md)
[^Math]: [Math](../static/Math.md)
[^Network]: [Network](../static/Network.md)
[^NetworkView]: [NetworkView](../objects/NetworkView.md)
[^PersistentData]: [PersistentData](../static/PersistentData.md)
[^Physics]: [Physics](../static/Physics.md)
[^Player]: [Player](../objects/Player.md)
[^Quaternion]: [Quaternion](../objects/Quaternion.md)
[^Random]: [Random](../objects/Random.md)
[^Range]: [Range](../objects/Range.md)
[^RoomData]: [RoomData](../static/RoomData.md)
[^Set]: [Set](../objects/Set.md)
[^Shifter]: [Shifter](../objects/Shifter.md)
[^String]: [String](../static/String.md)
[^Time]: [Time](../static/Time.md)
[^Titan]: [Titan](../objects/Titan.md)
[^Transform]: [Transform](../objects/Transform.md)
[^UI]: [UI](../static/UI.md)
[^Vector2]: [Vector2](../objects/Vector2.md)
[^Vector3]: [Vector3](../objects/Vector3.md)
[^Object]: [Object](../objects/Object.md)
[^Component]: [Component](../objects/Component.md)
