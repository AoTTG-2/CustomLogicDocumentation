# Network
Inherits from [Object](../md/objects/Object.md)

Networking functions.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|IsMasterClient|bool|True|Is the player the master client|
|Players|[List](../md/objects/List.md)|True|The list of players in the room|
|MasterClient|[Player](../md/objects/Player.md)|True|The master client|
|MyPlayer|[Player](../md/objects/Player.md)|True|The local player|
|NetworkTime|Double|True|The network time|
|Ping|int|True|The local player's ping|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function SendMessage(player: <a data-footnote-ref href="#user-content-fn-Player">Player</a>, message: string) -> null</code></pre>
> Send a message to a player

<pre class="language-typescript"><code class="lang-typescript">function SendMessageAll(message: string) -> null</code></pre>
> Send a message to all players

<pre class="language-typescript"><code class="lang-typescript">function SendMessageOthers(message: string) -> null</code></pre>
> Send a message to all players except the sender

<pre class="language-typescript"><code class="lang-typescript">function GetTimestampDifference(timestamp1: Double, timestamp2: Double) -> Double</code></pre>
> Get the difference between two photon timestamps

<pre class="language-typescript"><code class="lang-typescript">function KickPlayer(target: <a data-footnote-ref href="#user-content-fn-Object">Object</a>, [reason: string = .]) -> null</code></pre>
> Kick the given player by id or player reference.


[^Camera]: [Camera](../md/static/Camera.md)
[^Character]: [Character](../md/objects/Character.md)
[^Collider]: [Collider](../md/objects/Collider.md)
[^Collision]: [Collision](../md/objects/Collision.md)
[^Color]: [Color](../md/objects/Color.md)
[^Convert]: [Convert](../md/static/Convert.md)
[^Cutscene]: [Cutscene](../md/static/Cutscene.md)
[^Dict]: [Dict](../md/objects/Dict.md)
[^Game]: [Game](../md/static/Game.md)
[^Human]: [Human](../md/objects/Human.md)
[^Input]: [Input](../md/static/Input.md)
[^Json]: [Json](../md/static/Json.md)
[^LineCastHitResult]: [LineCastHitResult](../md/objects/LineCastHitResult.md)
[^LineRenderer]: [LineRenderer](../md/objects/LineRenderer.md)
[^List]: [List](../md/objects/List.md)
[^Map]: [Map](../md/static/Map.md)
[^MapObject]: [MapObject](../md/objects/MapObject.md)
[^MapTargetable]: [MapTargetable](../md/objects/MapTargetable.md)
[^Math]: [Math](../md/static/Math.md)
[^Network]: [Network](../md/static/Network.md)
[^NetworkView]: [NetworkView](../md/objects/NetworkView.md)
[^PersistentData]: [PersistentData](../md/static/PersistentData.md)
[^Physics]: [Physics](../md/static/Physics.md)
[^Player]: [Player](../md/objects/Player.md)
[^Quaternion]: [Quaternion](../md/objects/Quaternion.md)
[^Random]: [Random](../md/objects/Random.md)
[^Range]: [Range](../md/objects/Range.md)
[^RoomData]: [RoomData](../md/static/RoomData.md)
[^Set]: [Set](../md/objects/Set.md)
[^Shifter]: [Shifter](../md/objects/Shifter.md)
[^String]: [String](../md/static/String.md)
[^Time]: [Time](../md/static/Time.md)
[^Titan]: [Titan](../md/objects/Titan.md)
[^Transform]: [Transform](../md/objects/Transform.md)
[^UI]: [UI](../md/static/UI.md)
[^Vector2]: [Vector2](../md/objects/Vector2.md)
[^Vector3]: [Vector3](../md/objects/Vector3.md)
[^Object]: [Object](../md/objects/Object.md)
[^Component]: [Component](../md/objects/Component.md)
