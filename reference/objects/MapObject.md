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
#### <mark style="color:Blue;">CustomLogicComponentInstance</mark> <mark style="color:Yellow;">AddComponent</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">name</mark>)
Add a component to the object
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">RemoveComponent</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">name</mark>)
Remove a component from the object
#### <mark style="color:Blue;">CustomLogicComponentInstance</mark> <mark style="color:Yellow;">GetComponent</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">name</mark>)
Get a component from the object
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetComponentEnabled</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">name</mark>, <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">enabled</mark>)
Set whether a component is enabled
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetComponentsEnabled</mark>(<mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">enabled</mark>)
Set whether all components are enabled
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">AddSphereCollider</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">collideMode</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">collideWith</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">center</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">radius</mark>)
Add a sphere collider to the object
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">AddBoxCollider</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">collideMode</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">collideWith</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">center</mark> = <mark style="color:Blue;">null</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">size</mark> = <mark style="color:Blue;">null</mark>)
Add a box collider to the object
#### <mark style="color:Blue;">[MapTargetable](../objects/MapTargetable.md)</mark> <mark style="color:Yellow;">AddSphereTarget</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">team</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">center</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">radius</mark>)
Add a sphere target to the object
#### <mark style="color:Blue;">[MapTargetable](../objects/MapTargetable.md)</mark> <mark style="color:Yellow;">AddBoxTarget</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">team</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">center</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">size</mark>)
Add a box target to the object
#### <mark style="color:Blue;">[MapObject](../objects/MapObject.md)</mark> <mark style="color:Yellow;">GetChild</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">name</mark>)
Get a child object by name
#### <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">GetChildren</mark>()
Get all child objects
#### <mark style="color:Blue;">[Transform](../objects/Transform.md)</mark> <mark style="color:Yellow;">GetTransform</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">name</mark>)
Get a child transform by name
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetColorAll</mark>(<mark style="color:Blue;">[Color](../objects/Color.md)</mark> <mark style="color:Yellow;">color</mark>)
Set the color of all renderers on the object
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">InBounds</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">position</mark>)
Check if a position is within the object's bounds
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">GetBoundsAverageCenter</mark>()
Get the bounds average center
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">GetBoundsCenter</mark>()
Get the bounds center
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">GetBoundsSize</mark>()
Get the bounds size
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">GetBoundsMin</mark>()
Get the bounds min
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">GetBoundsMax</mark>()
Get the bounds max
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">GetBoundsExtents</mark>()
Get the bounds extents
#### <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">GetCorners</mark>()
Get the corners of the bounds
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">AddBuiltinComponent</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter0</mark> = <mark style="color:Blue;">null</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter1</mark> = <mark style="color:Blue;">null</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter2</mark> = <mark style="color:Blue;">null</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter3</mark> = <mark style="color:Blue;">null</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter4</mark> = <mark style="color:Blue;">null</mark>)
[OBSELETE] Add builtin component
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">HasTag</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">tag</mark>)
Whether or not the object has the given tag
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">ReadBuiltinComponent</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">name</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">param</mark>)
[OBSELETE] Read a builtin component
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">UpdateBuiltinComponent</mark>(<mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter0</mark> = <mark style="color:Blue;">null</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter1</mark> = <mark style="color:Blue;">null</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter2</mark> = <mark style="color:Blue;">null</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter3</mark> = <mark style="color:Blue;">null</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">parameter4</mark> = <mark style="color:Blue;">null</mark>)
[OBSELETE] Update a builtin component

---

