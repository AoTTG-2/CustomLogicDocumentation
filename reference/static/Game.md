# Game
Inherits from [Object](../objects/Object.md)

Game functions such as spawning titans and managing game state.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|IsEnding|bool|True|Is the game ending?|
|EndTimeLeft|float|True|Time left until the game ends|
|Titans|[List](../objects/List.md)|True|List of all titans|
|AITitans|[List](../objects/List.md)|True|List of all AI titans|
|PlayerTitans|[List](../objects/List.md)|True|List of all player titans|
|Shifters|[List](../objects/List.md)|True|List of all shifters|
|AIShifters|[List](../objects/List.md)|True|List of all AI shifters|
|PlayerShifters|[List](../objects/List.md)|True|List of all player shifters|
|Humans|[List](../objects/List.md)|True|List of all humans|
|AIHumans|[List](../objects/List.md)|True|List of all AI humans|
|PlayerHumans|[List](../objects/List.md)|True|List of all player humans|
|Loadouts|[List](../objects/List.md)|True|List of all loadouts|
|DefaultShowKillScore|bool|False|Is the kill score shown by default?|
|DefaultHideKillScore|bool|False|Is the kill feed shown by default?|
|DefaultAddKillScore|bool|False|Is the kill score added by default?|
|ShowScoreboardLoadout|bool|False|Is the loadout shown in the scoreboard?|
|ShowScoreboardStatus|bool|False|Is the status shown in the scoreboard?|
|ForcedCharacterType|string|False|Forced character type|
|ForcedLoadout|string|False|Forced loadout|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Debug(message: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Print a debug statement to the console

<pre class="language-typescript"><code class="lang-typescript">function Print(message: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Print a message to the chat

<pre class="language-typescript"><code class="lang-typescript">function PrintAll(message: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Print a message to all players

<pre class="language-typescript"><code class="lang-typescript">function GetGeneralSetting(settingName: string) -> <a data-footnote-ref href="#user-content-fn-Object">Object</a></code></pre>
> Get a general setting

<pre class="language-typescript"><code class="lang-typescript">function GetTitanSetting(settingName: string) -> <a data-footnote-ref href="#user-content-fn-Object">Object</a></code></pre>
> Get a titan setting

<pre class="language-typescript"><code class="lang-typescript">function GetMiscSetting(settingName: string) -> <a data-footnote-ref href="#user-content-fn-Object">Object</a></code></pre>
> Get a misc setting

<pre class="language-typescript"><code class="lang-typescript">function End(delay: float) -> null</code></pre>
> End the game

<pre class="language-typescript"><code class="lang-typescript">function FindCharacterByViewID(viewID: int) -> <a data-footnote-ref href="#user-content-fn-Character">Character</a></code></pre>
> Find a character by view ID

<pre class="language-typescript"><code class="lang-typescript">function SpawnTitan(type: string) -> <a data-footnote-ref href="#user-content-fn-Titan">Titan</a></code></pre>
> Spawn a titan

<pre class="language-typescript"><code class="lang-typescript">function SpawnTitanAt(type: string, position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [rotationY: float = 0]) -> <a data-footnote-ref href="#user-content-fn-Titan">Titan</a></code></pre>
> Spawn a titan at a position

<pre class="language-typescript"><code class="lang-typescript">function SpawnTitans(type: string, count: int) -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Spawn titans

<pre class="language-typescript"><code class="lang-typescript">function SpawnTitansAsync(type: string, count: int) -> null</code></pre>
> Spawn titans asynchronously

<pre class="language-typescript"><code class="lang-typescript">function SpawnTitansAt(type: string, count: int, position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [rotationY: float = 0]) -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Spawn titans at a position

<pre class="language-typescript"><code class="lang-typescript">function SpawnTitansAtAsync(type: string, count: int, position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [rotationY: float = 0]) -> null</code></pre>
> Spawn titans at a position asynchronously

<pre class="language-typescript"><code class="lang-typescript">function SpawnShifter(type: string) -> <a data-footnote-ref href="#user-content-fn-Shifter">Shifter</a></code></pre>
> Spawn a shifter

<pre class="language-typescript"><code class="lang-typescript">function SpawnShifterAt(type: string, position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [rotationY: float = 0]) -> <a data-footnote-ref href="#user-content-fn-Shifter">Shifter</a></code></pre>
> Spawn a shifter at a position

<pre class="language-typescript"><code class="lang-typescript">function SpawnProjectile(parameters: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Spawn a projectile

<pre class="language-typescript"><code class="lang-typescript">function SpawnProjectileWithOwner(parameters: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Spawn a projectile with an owner

<pre class="language-typescript"><code class="lang-typescript">function SpawnEffect(parameters: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Spawn an effect

<pre class="language-typescript"><code class="lang-typescript">function SpawnPlayer(player: <a data-footnote-ref href="#user-content-fn-Player">Player</a>, force: bool) -> null</code></pre>
> Spawn a player

<pre class="language-typescript"><code class="lang-typescript">function SpawnPlayerAll(force: bool) -> null</code></pre>
> Spawn a player for all players

<pre class="language-typescript"><code class="lang-typescript">function SpawnPlayerAt(player: <a data-footnote-ref href="#user-content-fn-Player">Player</a>, force: bool, position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [rotationY: float = 0]) -> null</code></pre>
> Spawn a player at a position

<pre class="language-typescript"><code class="lang-typescript">function SpawnPlayerAtAll(force: bool, position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [rotationY: float = 0]) -> null</code></pre>
> Spawn a player at a position for all players

<pre class="language-typescript"><code class="lang-typescript">function SetPlaylist(playlist: string) -> null</code></pre>
> Set the music playlist

<pre class="language-typescript"><code class="lang-typescript">function SetSong(song: string) -> null</code></pre>
> Set the music song

<pre class="language-typescript"><code class="lang-typescript">function DrawRay(start: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, dir: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, color: <a data-footnote-ref href="#user-content-fn-Color">Color</a>, duration: float) -> null</code></pre>
> Draw a ray

<pre class="language-typescript"><code class="lang-typescript">function ShowKillScore(damage: int) -> null</code></pre>
> Show the kill score

<pre class="language-typescript"><code class="lang-typescript">function ShowKillFeed(killer: string, victim: string, score: int, weapon: string) -> null</code></pre>
> Show the kill feed

<pre class="language-typescript"><code class="lang-typescript">function ShowKillFeedAll(killer: string, victim: string, score: int, weapon: string) -> null</code></pre>
> Show the kill feed for all players


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
