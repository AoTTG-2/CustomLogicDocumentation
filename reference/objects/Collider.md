# Collider
Inherits from [Object](../objects/Object.md)
### Remarks
Overloads operators: 
- `__Copy__`
- `==`
- `__Hash__`
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|AttachedArticulationBody|[Transform](../objects/Transform.md)|True||
|ContactOffset|float|False|Contact offset value of this collider.|
|Enabled|bool|False|Enabled Colliders will collide with other Colliders, disabled Colliders won't.|
|ExludeLayers|int|False|The additional layers that this Collider should exclude when deciding if the Collider can contact another Collider.|
|IncludeLayers|int|False|The additional layers that this Collider should include when deciding if the Collider can contact another Collider.|
|IsTrigger|bool|False|Specify if this collider is configured as a trigger.|
|Center|[Vector3](../objects/Vector3.md)|True|The center of the bounding box.|
|ProvidesContacts|bool|False|Whether or not this Collider generates contacts for Physics.ContactEvent.|
|MaterialName|string|True|The name of the physics material on the collider.|
|SharedMaterialName|string|True|The name of the shared physics material on this collider.|
|Transform|[Transform](../objects/Transform.md)|True|The collider's transform.|
|GameObjectTransform|[Transform](../objects/Transform.md)|True|The transform of the gameobject this collider is attached to.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function ClosestPoint(position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Returns a point on the collider that is closest to a given location.

> **Returns**: The point on the collider that is closest to the specified location.
<pre class="language-typescript"><code class="lang-typescript">function ClosestPointOnBounds(position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> The closest point to the bounding box of the attached collider.

<pre class="language-typescript"><code class="lang-typescript">function Raycast(start: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, maxDistance: float, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-LineCastHitResult">LineCastHitResult</a></code></pre>

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
