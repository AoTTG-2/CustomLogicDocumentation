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
#### <mark style="color:blue;">CustomLogicComponentInstance</mark> <mark style="color:yellow;">AddComponent</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> name)
> Add a component to the object
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">RemoveComponent</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> name)
> Remove a component from the object
#### <mark style="color:blue;">CustomLogicComponentInstance</mark> <mark style="color:yellow;">GetComponent</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> name)
> Get a component from the object
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetComponentEnabled</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> name, <mark style="color:blue;">bool</mark> enabled)
> Set whether a component is enabled
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetComponentsEnabled</mark>(<mark style="color:blue;">bool</mark> enabled)
> Set whether all components are enabled
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">AddSphereCollider</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> collideMode, <mark style="color:blue;">[String](../static/String.md)</mark> collideWith, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> center, <mark style="color:blue;">float</mark> radius)
> Add a sphere collider to the object
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">AddBoxCollider</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> collideMode, <mark style="color:blue;">[String](../static/String.md)</mark> collideWith, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> center = <mark style="color:blue;">null</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> size = <mark style="color:blue;">null</mark>)
> Add a box collider to the object
#### <mark style="color:blue;">[MapTargetable](../objects/MapTargetable.md)</mark> <mark style="color:yellow;">AddSphereTarget</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> team, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> center, <mark style="color:blue;">float</mark> radius)
> Add a sphere target to the object
#### <mark style="color:blue;">[MapTargetable](../objects/MapTargetable.md)</mark> <mark style="color:yellow;">AddBoxTarget</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> team, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> center, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> size)
> Add a box target to the object
#### <mark style="color:blue;">[MapObject](../objects/MapObject.md)</mark> <mark style="color:yellow;">GetChild</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> name)
> Get a child object by name
#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">GetChildren</mark>()
> Get all child objects
#### <mark style="color:blue;">[Transform](../objects/Transform.md)</mark> <mark style="color:yellow;">GetTransform</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> name)
> Get a child transform by name
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetColorAll</mark>(<mark style="color:blue;">[Color](../objects/Color.md)</mark> color)
> Set the color of all renderers on the object
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">InBounds</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> position)
> Check if a position is within the object's bounds
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">GetBoundsAverageCenter</mark>()
> Get the bounds average center
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">GetBoundsCenter</mark>()
> Get the bounds center
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">GetBoundsSize</mark>()
> Get the bounds size
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">GetBoundsMin</mark>()
> Get the bounds min
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">GetBoundsMax</mark>()
> Get the bounds max
#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">GetBoundsExtents</mark>()
> Get the bounds extents
#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">GetCorners</mark>()
> Get the corners of the bounds
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">AddBuiltinComponent</mark>(<mark style="color:blue;">Object</mark> parameter0 = <mark style="color:blue;">null</mark>, <mark style="color:blue;">Object</mark> parameter1 = <mark style="color:blue;">null</mark>, <mark style="color:blue;">Object</mark> parameter2 = <mark style="color:blue;">null</mark>, <mark style="color:blue;">Object</mark> parameter3 = <mark style="color:blue;">null</mark>, <mark style="color:blue;">Object</mark> parameter4 = <mark style="color:blue;">null</mark>)
> [OBSELETE] Add builtin component
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">HasTag</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> tag)
> Whether or not the object has the given tag
#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">ReadBuiltinComponent</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> name, <mark style="color:blue;">[String](../static/String.md)</mark> param)
> [OBSELETE] Read a builtin component
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">UpdateBuiltinComponent</mark>(<mark style="color:blue;">Object</mark> parameter0 = <mark style="color:blue;">null</mark>, <mark style="color:blue;">Object</mark> parameter1 = <mark style="color:blue;">null</mark>, <mark style="color:blue;">Object</mark> parameter2 = <mark style="color:blue;">null</mark>, <mark style="color:blue;">Object</mark> parameter3 = <mark style="color:blue;">null</mark>, <mark style="color:blue;">Object</mark> parameter4 = <mark style="color:blue;">null</mark>)
> [OBSELETE] Update a builtin component

---

