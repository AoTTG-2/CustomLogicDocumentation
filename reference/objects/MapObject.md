# MapObject
Inherits from [Object](../objects/Object.md)

MapObject represents a map object created in the editor or spawned at runtime using Map static methods.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Static|bool|True|Object does not move|
|Position|[Vector3](../objects/Vector3.md)|False|The position of the object|
|LocalPosition|[Vector3](../objects/Vector3.md)|False|The local position of the object|
|Rotation|[Vector3](../objects/Vector3.md)|False|The rotation of the object|
|LocalRotation|[Vector3](../objects/Vector3.md)|False|The local rotation of the object|
|QuaternionRotation|[Quaternion](../objects/Quaternion.md)|False|The rotation of the object as a quaternion|
|QuaternionLocalRotation|[Quaternion](../objects/Quaternion.md)|False|The local rotation of the object as a quaternion|
|Forward|[Vector3](../objects/Vector3.md)|False|The forward direction of the object|
|Up|[Vector3](../objects/Vector3.md)|False|The up direction of the object|
|Right|[Vector3](../objects/Vector3.md)|False|The right direction of the object|
|Scale|[Vector3](../objects/Vector3.md)|False|The scale of the object|
|Name|string|True|The name of the object|
|Parent|[Object](../objects/Object.md)|False|The parent of the object|
|Active|bool|False|Whether the object is active|
|Transform|[Transform](../objects/Transform.md)|True|The transform of the object|
|HasRenderer|bool|True|Whether the object has a renderer|
|Color|[Color](../objects/Color.md)|False|The color of the object|
|TextureTilingX|float|False|The x tiling of the object's texture|
|TextureTilingY|float|False|The y tiling of the object's texture|
|TextureOffsetX|float|False|The x offset of the object's texture|
|TextureOffsetY|float|False|The y offset of the object's texture|
|ID|int|True|The ID of the object|
|Tag|string|False|The tag of the object|
|Layer|int|False|The layer of the object|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function AddComponent(name: string) -> component</code></pre>
> Add a component to the object

<pre class="language-typescript"><code class="lang-typescript">function RemoveComponent(name: string) -> null</code></pre>
> Remove a component from the object

<pre class="language-typescript"><code class="lang-typescript">function GetComponent(name: string) -> component</code></pre>
> Get a component from the object

<pre class="language-typescript"><code class="lang-typescript">function SetComponentEnabled(name: string, enabled: bool) -> null</code></pre>
> Set whether a component is enabled

<pre class="language-typescript"><code class="lang-typescript">function SetComponentsEnabled(enabled: bool) -> null</code></pre>
> Set whether all components are enabled

<pre class="language-typescript"><code class="lang-typescript">function AddSphereCollider(collideMode: string, collideWith: string, center: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, radius: float) -> null</code></pre>
> Add a sphere collider to the object

<pre class="language-typescript"><code class="lang-typescript">function AddBoxCollider(collideMode: string, collideWith: string, [center: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a> = null], [size: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a> = null]) -> null</code></pre>
> Add a box collider to the object

<pre class="language-typescript"><code class="lang-typescript">function AddSphereTarget(team: string, center: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, radius: float) -> <a data-footnote-ref href="#user-content-fn-MapTargetable">MapTargetable</a></code></pre>
> Add a sphere target to the object

<pre class="language-typescript"><code class="lang-typescript">function AddBoxTarget(team: string, center: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, size: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-MapTargetable">MapTargetable</a></code></pre>
> Add a box target to the object

<pre class="language-typescript"><code class="lang-typescript">function GetChild(name: string) -> <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a></code></pre>
> Get a child object by name

<pre class="language-typescript"><code class="lang-typescript">function GetChildren() -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Get all child objects

<pre class="language-typescript"><code class="lang-typescript">function GetTransform(name: string) -> <a data-footnote-ref href="#user-content-fn-Transform">Transform</a></code></pre>
> Get a child transform by name

<pre class="language-typescript"><code class="lang-typescript">function SetColorAll(color: <a data-footnote-ref href="#user-content-fn-Color">Color</a>) -> null</code></pre>
> Set the color of all renderers on the object

<pre class="language-typescript"><code class="lang-typescript">function InBounds(position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> bool</code></pre>
> Check if a position is within the object's bounds

<pre class="language-typescript"><code class="lang-typescript">function GetBoundsAverageCenter() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Get the bounds average center

<pre class="language-typescript"><code class="lang-typescript">function GetBoundsCenter() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Get the bounds center

<pre class="language-typescript"><code class="lang-typescript">function GetBoundsSize() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Get the bounds size

<pre class="language-typescript"><code class="lang-typescript">function GetBoundsMin() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Get the bounds min

<pre class="language-typescript"><code class="lang-typescript">function GetBoundsMax() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Get the bounds max

<pre class="language-typescript"><code class="lang-typescript">function GetBoundsExtents() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Get the bounds extents

<pre class="language-typescript"><code class="lang-typescript">function GetCorners() -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Get the corners of the bounds

<pre class="language-typescript"><code class="lang-typescript">function AddBuiltinComponent([componentName: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null], [parameter1: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null], [parameter2: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null], [parameter3: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null], [parameter4: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null]) -> null</code></pre>
> Add a builtin component to the object.
Components: Daylight, PointLight, Tag, Rigidbody, CustomPhysicsMaterial, NavMeshObstacle

<pre class="language-typescript"><code class="lang-typescript">function HasTag(tag: string) -> bool</code></pre>
> Whether or not the object has the given tag

<pre class="language-typescript"><code class="lang-typescript">function ReadBuiltinComponent(name: string, param: string) -> <a data-footnote-ref href="#user-content-fn-Object">Object</a></code></pre>
> Read a builtin component

<pre class="language-typescript"><code class="lang-typescript">function UpdateBuiltinComponent([componentName: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null], [parameter1: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null], [parameter2: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null], [parameter3: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null], [parameter4: <a data-footnote-ref href="#user-content-fn-Object">Object</a> = null]) -> null</code></pre>
> Update a builtin component


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
