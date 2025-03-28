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
#### <span style="color:#509cd4;">CustomLogicComponentInstance</span> <span style="color:#dcdcaa;">AddComponent</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">name</span>)
Add a component to the object
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">RemoveComponent</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">name</span>)
Remove a component from the object
#### <span style="color:#509cd4;">CustomLogicComponentInstance</span> <span style="color:#dcdcaa;">GetComponent</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">name</span>)
Get a component from the object
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetComponentEnabled</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">name</span>, <span style="color:#509cd4;">bool</span> <span style="color:#9cdcfe;">enabled</span>)
Set whether a component is enabled
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetComponentsEnabled</span>(<span style="color:#509cd4;">bool</span> <span style="color:#9cdcfe;">enabled</span>)
Set whether all components are enabled
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">AddSphereCollider</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">collideMode</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">collideWith</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">center</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">radius</span>)
Add a sphere collider to the object
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">AddBoxCollider</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">collideMode</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">collideWith</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">center</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">size</span> = <span style="color:#509cd4;">null</span>)
Add a box collider to the object
#### <span style="color:#509cd4;">[MapTargetable](../objects/MapTargetable.md)</span> <span style="color:#dcdcaa;">AddSphereTarget</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">team</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">center</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">radius</span>)
Add a sphere target to the object
#### <span style="color:#509cd4;">[MapTargetable](../objects/MapTargetable.md)</span> <span style="color:#dcdcaa;">AddBoxTarget</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">team</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">center</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">size</span>)
Add a box target to the object
#### <span style="color:#509cd4;">[MapObject](../objects/MapObject.md)</span> <span style="color:#dcdcaa;">GetChild</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">name</span>)
Get a child object by name
#### <span style="color:#509cd4;">[List](../objects/List.md)</span> <span style="color:#dcdcaa;">GetChildren</span>()
Get all child objects
#### <span style="color:#509cd4;">[Transform](../objects/Transform.md)</span> <span style="color:#dcdcaa;">GetTransform</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">name</span>)
Get a child transform by name
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetColorAll</span>(<span style="color:#509cd4;">[Color](../objects/Color.md)</span> <span style="color:#9cdcfe;">color</span>)
Set the color of all renderers on the object
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">InBounds</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">position</span>)
Check if a position is within the object's bounds
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">GetBoundsAverageCenter</span>()
Get the bounds average center
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">GetBoundsCenter</span>()
Get the bounds center
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">GetBoundsSize</span>()
Get the bounds size
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">GetBoundsMin</span>()
Get the bounds min
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">GetBoundsMax</span>()
Get the bounds max
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">GetBoundsExtents</span>()
Get the bounds extents
#### <span style="color:#509cd4;">[List](../objects/List.md)</span> <span style="color:#dcdcaa;">GetCorners</span>()
Get the corners of the bounds
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">AddBuiltinComponent</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter0</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter1</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter2</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter3</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter4</span> = <span style="color:#509cd4;">null</span>)
[OBSELETE] Add builtin component
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">HasTag</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">tag</span>)
Whether or not the object has the given tag
#### <span style="color:#509cd4;">Object</span> <span style="color:#dcdcaa;">ReadBuiltinComponent</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">name</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">param</span>)
[OBSELETE] Read a builtin component
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">UpdateBuiltinComponent</span>(<span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter0</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter1</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter2</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter3</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">parameter4</span> = <span style="color:#509cd4;">null</span>)
[OBSELETE] Update a builtin component

---

