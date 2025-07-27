# MapTargetable
Inherits from [Object](../objects/Object.md)

MapTargetable object returned from MapObject.AddTarget method.
Creating a map targetable is similar to adding a collider to the MapObject,
except this collider can be targeted by AI such as titans.
Map targetables that are on a different team than the AI will be targeted by the titan,
and will trigger the OnGetHit callback on the attached MapObject.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Team|string|False|The team of the targetable|
|Position|[Vector3](../objects/Vector3.md)|True|The position of the targetable|
|Enabled|bool|False|Is the targetable enabled|


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
