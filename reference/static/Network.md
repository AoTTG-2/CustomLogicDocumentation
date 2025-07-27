# Network
Inherits from [Object](../objects/Object.md)

Networking functions.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|IsMasterClient|bool|True|Is the player the master client|
|Players|[List](../objects/List.md)|True|The list of players in the room|
|MasterClient|[Player](../objects/Player.md)|True|The master client|
|MyPlayer|[Player](../objects/Player.md)|True|The local player|
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
