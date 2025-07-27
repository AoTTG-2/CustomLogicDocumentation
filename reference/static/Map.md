# Map
Inherits from [Object](../objects/Object.md)

Finding, creating, and destroying map objects.

### Methods
<pre class="language-typescript"><code class="lang-typescript">function FindAllMapObjects() -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Find all map objects

<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectByName(objectName: string) -> <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a></code></pre>
> Find a map object by name

<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectsByName(objectName: string) -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Find all map objects by name

<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectByComponent(className: string) -> <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a></code></pre>
> Find all map objects by component

<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectsByComponent(className: string) -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Find all map objects by component

<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectByID(id: int) -> <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a></code></pre>
> Find a map object by ID

<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectByTag(tag: string) -> <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a></code></pre>
> Find a map object by tag

<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectsByTag(tag: string) -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Find all map objects by tag

<pre class="language-typescript"><code class="lang-typescript">function CreateMapObjectRaw(prefab: string) -> <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a></code></pre>
> Create a new map object

<pre class="language-typescript"><code class="lang-typescript">function DestroyMapObject(mapObject: <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a>, includeChildren: bool) -> null</code></pre>
> Destroy a map object

<pre class="language-typescript"><code class="lang-typescript">function CopyMapObject(mapObject: <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a>, includeChildren: bool) -> <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a></code></pre>
> Copy a map object

<pre class="language-typescript"><code class="lang-typescript">function DestroyMapTargetable(targetable: <a data-footnote-ref href="#user-content-fn-MapTargetable">MapTargetable</a>) -> null</code></pre>
> Destroy a map targetable

<pre class="language-typescript"><code class="lang-typescript">function UpdateNavMesh() -> null</code></pre>
> Update the nav mesh

<pre class="language-typescript"><code class="lang-typescript">function UpdateNavMeshAsync() -> null</code></pre>
> Update the nav mesh asynchronously


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
