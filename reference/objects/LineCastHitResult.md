# LineCastHitResult
Inherits from object
## Fields
|<div style="width:30%">Field</div>|<div style="width:10%">Type</div>|<div style="width:10%">Readonly</div>|<div style="width:50%">Description</div>|
|---|---|---|---|
|IsCharacter|bool|True|true if the linecast hit a character|
|IsMapObject|bool|True|true if the linecast hit a map object|
|Distance|float|True|The distance to the hit point|
|Point|[Vector3](../objects/Vector3.md)|True|The point in world space where the linecast hit|
|Normal|[Vector3](../objects/Vector3.md)|True|The normal of the surface the linecast hit|
|Collider|[Collider](../objects/Collider.md)|True|The collider that was hit|
