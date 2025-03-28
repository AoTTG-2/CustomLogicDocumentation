# MapObject
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Static|bool|False|Object does not move|
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
|Name|[String](../static/String.md)|False|The name of the object|
|Parent|Object|False|The parent of the object|
|Active|bool|False|Whether the object is active|
|Transform|[Transform](../objects/Transform.md)|False|The transform of the object|
|HasRenderer|bool|False|Whether the object has a renderer|
|Color|[Color](../objects/Color.md)|False|The color of the object|
|TextureTilingX|float|False|The x tiling of the object's texture|
|TextureTilingY|float|False|The y tiling of the object's texture|
|TextureOffsetX|float|False|The x offset of the object's texture|
|TextureOffsetY|float|False|The y offset of the object's texture|
|ID|int|False|The ID of the object|
|Tag|[String](../static/String.md)|False|The tag of the object|
|Layer|int|False|The layer of the object|
## Methods
#### <mark style="color:#509cd4;">CustomLogicComponentInstance</mark> <mark style="color:#dcdcaa;">AddComponent</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">name</mark>)
Add a component to the object
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">RemoveComponent</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">name</mark>)
Remove a component from the object
#### <mark style="color:#509cd4;">CustomLogicComponentInstance</mark> <mark style="color:#dcdcaa;">GetComponent</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">name</mark>)
Get a component from the object
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetComponentEnabled</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">name</mark>, <mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">enabled</mark>)
Set whether a component is enabled
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetComponentsEnabled</mark>(<mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">enabled</mark>)
Set whether all components are enabled
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">AddSphereCollider</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">collideMode</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">collideWith</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">center</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">radius</mark>)
Add a sphere collider to the object
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">AddBoxCollider</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">collideMode</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">collideWith</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">center</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">size</mark> = <mark style="color:#509cd4;">null</mark>)
Add a box collider to the object
#### <mark style="color:#509cd4;">[MapTargetable](../objects/MapTargetable.md)</mark> <mark style="color:#dcdcaa;">AddSphereTarget</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">team</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">center</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">radius</mark>)
Add a sphere target to the object
#### <mark style="color:#509cd4;">[MapTargetable](../objects/MapTargetable.md)</mark> <mark style="color:#dcdcaa;">AddBoxTarget</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">team</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">center</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">size</mark>)
Add a box target to the object
#### <mark style="color:#509cd4;">[MapObject](../objects/MapObject.md)</mark> <mark style="color:#dcdcaa;">GetChild</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">name</mark>)
Get a child object by name
#### <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#dcdcaa;">GetChildren</mark>()
Get all child objects
#### <mark style="color:#509cd4;">[Transform](../objects/Transform.md)</mark> <mark style="color:#dcdcaa;">GetTransform</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">name</mark>)
Get a child transform by name
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetColorAll</mark>(<mark style="color:#509cd4;">[Color](../objects/Color.md)</mark> <mark style="color:#9cdcfe;">color</mark>)
Set the color of all renderers on the object
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">InBounds</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>)
Check if a position is within the object's bounds
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">GetBoundsAverageCenter</mark>()
Get the bounds average center
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">GetBoundsCenter</mark>()
Get the bounds center
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">GetBoundsSize</mark>()
Get the bounds size
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">GetBoundsMin</mark>()
Get the bounds min
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">GetBoundsMax</mark>()
Get the bounds max
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">GetBoundsExtents</mark>()
Get the bounds extents
#### <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#dcdcaa;">GetCorners</mark>()
Get the corners of the bounds
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">AddBuiltinComponent</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter0</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter1</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter2</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter3</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter4</mark> = <mark style="color:#509cd4;">null</mark>)
[OBSELETE] Add builtin component
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">HasTag</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">tag</mark>)
Whether or not the object has the given tag
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">ReadBuiltinComponent</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">name</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">param</mark>)
[OBSELETE] Read a builtin component
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">UpdateBuiltinComponent</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter0</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter1</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter2</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter3</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">parameter4</mark> = <mark style="color:#509cd4;">null</mark>)
[OBSELETE] Update a builtin component

---

