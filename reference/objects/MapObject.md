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
|Function|Returns|Description|
|---|---|---|
|AddComponent(<i>name</i> : [String](../static/String.md))|CustomLogicComponentInstance|Add a component to the object|
|RemoveComponent(<i>name</i> : [String](../static/String.md))|none|Remove a component from the object|
|GetComponent(<i>name</i> : [String](../static/String.md))|CustomLogicComponentInstance|Get a component from the object|
|SetComponentEnabled(<br/><i>name</i> : [String](../static/String.md),<br/><i>enabled</i> : bool<br/>)|none|Set whether a component is enabled|
|SetComponentsEnabled(<i>enabled</i> : bool)|none|Set whether all components are enabled|
|AddSphereCollider(<br/><i>collideMode</i> : [String](../static/String.md),<br/><i>collideWith</i> : [String](../static/String.md),<br/><i>center</i> : [Vector3](../objects/Vector3.md),<br/><i>radius</i> : float<br/>)|none|Add a sphere collider to the object|
|AddBoxCollider(<br/><i>collideMode</i> : [String](../static/String.md),<br/><i>collideWith</i> : [String](../static/String.md),<br/><i>center</i> : [Vector3](../objects/Vector3.md) = ,<br/><i>size</i> : [Vector3](../objects/Vector3.md) = <br/>)|none|Add a box collider to the object|
|AddSphereTarget(<br/><i>team</i> : [String](../static/String.md),<br/><i>center</i> : [Vector3](../objects/Vector3.md),<br/><i>radius</i> : float<br/>)|[MapTargetable](../objects/MapTargetable.md)|Add a sphere target to the object|
|AddBoxTarget(<br/><i>team</i> : [String](../static/String.md),<br/><i>center</i> : [Vector3](../objects/Vector3.md),<br/><i>size</i> : [Vector3](../objects/Vector3.md)<br/>)|[MapTargetable](../objects/MapTargetable.md)|Add a box target to the object|
|GetChild(<i>name</i> : [String](../static/String.md))|[MapObject](../objects/MapObject.md)|Get a child object by name|
|GetChildren()|[List](../objects/List.md)|Get all child objects|
|GetTransform(<i>name</i> : [String](../static/String.md))|[Transform](../objects/Transform.md)|Get a child transform by name|
|SetColorAll(<i>color</i> : [Color](../objects/Color.md))|none|Set the color of all renderers on the object|
|InBounds(<i>position</i> : [Vector3](../objects/Vector3.md))|bool|Check if a position is within the object's bounds|
|GetBoundsAverageCenter()|[Vector3](../objects/Vector3.md)|Get the bounds average center|
|GetBoundsCenter()|[Vector3](../objects/Vector3.md)|Get the bounds center|
|GetBoundsSize()|[Vector3](../objects/Vector3.md)|Get the bounds size|
|GetBoundsMin()|[Vector3](../objects/Vector3.md)|Get the bounds min|
|GetBoundsMax()|[Vector3](../objects/Vector3.md)|Get the bounds max|
|GetBoundsExtents()|[Vector3](../objects/Vector3.md)|Get the bounds extents|
|GetCorners()|[List](../objects/List.md)|Get the corners of the bounds|
|AddBuiltinComponent(<br/><i>parameter0</i> : Object = ,<br/><i>parameter1</i> : Object = ,<br/><i>parameter2</i> : Object = ,<br/><i>parameter3</i> : Object = ,<br/><i>parameter4</i> : Object = <br/>)|none|[OBSELETE] Add builtin component|
|ReadBuiltinComponent(<br/><i>name</i> : [String](../static/String.md),<br/><i>param</i> : [String](../static/String.md)<br/>)|Object|[OBSELETE] Read a builtin component|
|UpdateBuiltinComponent(<br/><i>parameter0</i> : Object = ,<br/><i>parameter1</i> : Object = ,<br/><i>parameter2</i> : Object = ,<br/><i>parameter3</i> : Object = ,<br/><i>parameter4</i> : Object = <br/>)|none|[OBSELETE] Update a builtin component|
