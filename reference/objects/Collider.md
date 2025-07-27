# Collider
Inherits from [Object](../md/objects/Object.md)
### Remarks
Overloads operators: 
- `__Copy__`
- `==`
- `__Hash__`
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|AttachedArticulationBody|[Transform](../md/objects/Transform.md)|True||
|ContactOffset|float|False|Contact offset value of this collider.|
|Enabled|bool|False|Enabled Colliders will collide with other Colliders, disabled Colliders won't.|
|ExludeLayers|int|False|The additional layers that this Collider should exclude when deciding if the Collider can contact another Collider.|
|IncludeLayers|int|False|The additional layers that this Collider should include when deciding if the Collider can contact another Collider.|
|IsTrigger|bool|False|Specify if this collider is configured as a trigger.|
|Center|[Vector3](../md/objects/Vector3.md)|True|The center of the bounding box.|
|ProvidesContacts|bool|False|Whether or not this Collider generates contacts for Physics.ContactEvent.|
|MaterialName|string|True|The name of the physics material on the collider.|
|SharedMaterialName|string|True|The name of the shared physics material on this collider.|
|Transform|[Transform](../md/objects/Transform.md)|True|The collider's transform.|
|GameObjectTransform|[Transform](../md/objects/Transform.md)|True|The transform of the gameobject this collider is attached to.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function ClosestPoint(position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Returns a point on the collider that is closest to a given location.

> **Returns**: The point on the collider that is closest to the specified location.
<pre class="language-typescript"><code class="lang-typescript">function ClosestPointOnBounds(position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> The closest point to the bounding box of the attached collider.

<pre class="language-typescript"><code class="lang-typescript">function Raycast(start: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, maxDistance: float, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-LineCastHitResult">LineCastHitResult</a></code></pre>

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
