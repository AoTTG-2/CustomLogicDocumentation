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
#### CustomLogicComponentInstance <span style="color":#dcdcaa>AddComponent<span>([String](../static/String.md) <span style="color":#9cdcfe>name<span>)
Add a component to the object
#### void <span style="color":#dcdcaa>RemoveComponent<span>([String](../static/String.md) <span style="color":#9cdcfe>name<span>)
Remove a component from the object
#### CustomLogicComponentInstance <span style="color":#dcdcaa>GetComponent<span>([String](../static/String.md) <span style="color":#9cdcfe>name<span>)
Get a component from the object
#### void <span style="color":#dcdcaa>SetComponentEnabled<span>([String](../static/String.md) <span style="color":#9cdcfe>name<span>, bool <span style="color":#9cdcfe>enabled<span>)
Set whether a component is enabled
#### void <span style="color":#dcdcaa>SetComponentsEnabled<span>(bool <span style="color":#9cdcfe>enabled<span>)
Set whether all components are enabled
#### void <span style="color":#dcdcaa>AddSphereCollider<span>([String](../static/String.md) <span style="color":#9cdcfe>collideMode<span>, [String](../static/String.md) <span style="color":#9cdcfe>collideWith<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>center<span>, float <span style="color":#9cdcfe>radius<span>)
Add a sphere collider to the object
#### void <span style="color":#dcdcaa>AddBoxCollider<span>([String](../static/String.md) <span style="color":#9cdcfe>collideMode<span>, [String](../static/String.md) <span style="color":#9cdcfe>collideWith<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>center<span> = null, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>size<span> = null)
Add a box collider to the object
#### [MapTargetable](../objects/MapTargetable.md) <span style="color":#dcdcaa>AddSphereTarget<span>([String](../static/String.md) <span style="color":#9cdcfe>team<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>center<span>, float <span style="color":#9cdcfe>radius<span>)
Add a sphere target to the object
#### [MapTargetable](../objects/MapTargetable.md) <span style="color":#dcdcaa>AddBoxTarget<span>([String](../static/String.md) <span style="color":#9cdcfe>team<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>center<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>size<span>)
Add a box target to the object
#### [MapObject](../objects/MapObject.md) <span style="color":#dcdcaa>GetChild<span>([String](../static/String.md) <span style="color":#9cdcfe>name<span>)
Get a child object by name
#### [List](../objects/List.md) <span style="color":#dcdcaa>GetChildren<span>()
Get all child objects
#### [Transform](../objects/Transform.md) <span style="color":#dcdcaa>GetTransform<span>([String](../static/String.md) <span style="color":#9cdcfe>name<span>)
Get a child transform by name
#### void <span style="color":#dcdcaa>SetColorAll<span>([Color](../objects/Color.md) <span style="color":#9cdcfe>color<span>)
Set the color of all renderers on the object
#### bool <span style="color":#dcdcaa>InBounds<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>)
Check if a position is within the object's bounds
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>GetBoundsAverageCenter<span>()
Get the bounds average center
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>GetBoundsCenter<span>()
Get the bounds center
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>GetBoundsSize<span>()
Get the bounds size
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>GetBoundsMin<span>()
Get the bounds min
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>GetBoundsMax<span>()
Get the bounds max
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>GetBoundsExtents<span>()
Get the bounds extents
#### [List](../objects/List.md) <span style="color":#dcdcaa>GetCorners<span>()
Get the corners of the bounds
#### void <span style="color":#dcdcaa>AddBuiltinComponent<span>(Object <span style="color":#9cdcfe>parameter0<span> = null, Object <span style="color":#9cdcfe>parameter1<span> = null, Object <span style="color":#9cdcfe>parameter2<span> = null, Object <span style="color":#9cdcfe>parameter3<span> = null, Object <span style="color":#9cdcfe>parameter4<span> = null)
[OBSELETE] Add builtin component
#### bool <span style="color":#dcdcaa>HasTag<span>([String](../static/String.md) <span style="color":#9cdcfe>tag<span>)
Whether or not the object has the given tag
#### Object <span style="color":#dcdcaa>ReadBuiltinComponent<span>([String](../static/String.md) <span style="color":#9cdcfe>name<span>, [String](../static/String.md) <span style="color":#9cdcfe>param<span>)
[OBSELETE] Read a builtin component
#### void <span style="color":#dcdcaa>UpdateBuiltinComponent<span>(Object <span style="color":#9cdcfe>parameter0<span> = null, Object <span style="color":#9cdcfe>parameter1<span> = null, Object <span style="color":#9cdcfe>parameter2<span> = null, Object <span style="color":#9cdcfe>parameter3<span> = null, Object <span style="color":#9cdcfe>parameter4<span> = null)
[OBSELETE] Update a builtin component

---

