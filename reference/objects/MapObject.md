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
#### <span style="color:blue;">CustomLogicComponentInstance</span> <span style="color:yellow;">AddComponent</span>(<span style="color:blue;">[String](../static/String.md)</span> name)
> Add a component to the object
#### <span style="color:blue;">void</span> <span style="color:yellow;">RemoveComponent</span>(<span style="color:blue;">[String](../static/String.md)</span> name)
> Remove a component from the object
#### <span style="color:blue;">CustomLogicComponentInstance</span> <span style="color:yellow;">GetComponent</span>(<span style="color:blue;">[String](../static/String.md)</span> name)
> Get a component from the object
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetComponentEnabled</span>(<span style="color:blue;">[String](../static/String.md)</span> name, <span style="color:blue;">bool</span> enabled)
> Set whether a component is enabled
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetComponentsEnabled</span>(<span style="color:blue;">bool</span> enabled)
> Set whether all components are enabled
#### <span style="color:blue;">void</span> <span style="color:yellow;">AddSphereCollider</span>(<span style="color:blue;">[String](../static/String.md)</span> collideMode, <span style="color:blue;">[String](../static/String.md)</span> collideWith, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> center, <span style="color:blue;">float</span> radius)
> Add a sphere collider to the object
#### <span style="color:blue;">void</span> <span style="color:yellow;">AddBoxCollider</span>(<span style="color:blue;">[String](../static/String.md)</span> collideMode, <span style="color:blue;">[String](../static/String.md)</span> collideWith, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> center = <span style="color:blue;">null</span>, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> size = <span style="color:blue;">null</span>)
> Add a box collider to the object
#### <span style="color:blue;">[MapTargetable](../objects/MapTargetable.md)</span> <span style="color:yellow;">AddSphereTarget</span>(<span style="color:blue;">[String](../static/String.md)</span> team, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> center, <span style="color:blue;">float</span> radius)
> Add a sphere target to the object
#### <span style="color:blue;">[MapTargetable](../objects/MapTargetable.md)</span> <span style="color:yellow;">AddBoxTarget</span>(<span style="color:blue;">[String](../static/String.md)</span> team, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> center, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> size)
> Add a box target to the object
#### <span style="color:blue;">[MapObject](../objects/MapObject.md)</span> <span style="color:yellow;">GetChild</span>(<span style="color:blue;">[String](../static/String.md)</span> name)
> Get a child object by name
#### <span style="color:blue;">[List](../objects/List.md)</span> <span style="color:yellow;">GetChildren</span>()
> Get all child objects
#### <span style="color:blue;">[Transform](../objects/Transform.md)</span> <span style="color:yellow;">GetTransform</span>(<span style="color:blue;">[String](../static/String.md)</span> name)
> Get a child transform by name
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetColorAll</span>(<span style="color:blue;">[Color](../objects/Color.md)</span> color)
> Set the color of all renderers on the object
#### <span style="color:blue;">bool</span> <span style="color:yellow;">InBounds</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position)
> Check if a position is within the object's bounds
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">GetBoundsAverageCenter</span>()
> Get the bounds average center
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">GetBoundsCenter</span>()
> Get the bounds center
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">GetBoundsSize</span>()
> Get the bounds size
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">GetBoundsMin</span>()
> Get the bounds min
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">GetBoundsMax</span>()
> Get the bounds max
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">GetBoundsExtents</span>()
> Get the bounds extents
#### <span style="color:blue;">[List](../objects/List.md)</span> <span style="color:yellow;">GetCorners</span>()
> Get the corners of the bounds
#### <span style="color:blue;">void</span> <span style="color:yellow;">AddBuiltinComponent</span>(<span style="color:blue;">Object</span> parameter0 = <span style="color:blue;">null</span>, <span style="color:blue;">Object</span> parameter1 = <span style="color:blue;">null</span>, <span style="color:blue;">Object</span> parameter2 = <span style="color:blue;">null</span>, <span style="color:blue;">Object</span> parameter3 = <span style="color:blue;">null</span>, <span style="color:blue;">Object</span> parameter4 = <span style="color:blue;">null</span>)
> [OBSELETE] Add builtin component
#### <span style="color:blue;">bool</span> <span style="color:yellow;">HasTag</span>(<span style="color:blue;">[String](../static/String.md)</span> tag)
> Whether or not the object has the given tag
#### <span style="color:blue;">Object</span> <span style="color:yellow;">ReadBuiltinComponent</span>(<span style="color:blue;">[String](../static/String.md)</span> name, <span style="color:blue;">[String](../static/String.md)</span> param)
> [OBSELETE] Read a builtin component
#### <span style="color:blue;">void</span> <span style="color:yellow;">UpdateBuiltinComponent</span>(<span style="color:blue;">Object</span> parameter0 = <span style="color:blue;">null</span>, <span style="color:blue;">Object</span> parameter1 = <span style="color:blue;">null</span>, <span style="color:blue;">Object</span> parameter2 = <span style="color:blue;">null</span>, <span style="color:blue;">Object</span> parameter3 = <span style="color:blue;">null</span>, <span style="color:blue;">Object</span> parameter4 = <span style="color:blue;">null</span>)
> [OBSELETE] Update a builtin component

---

