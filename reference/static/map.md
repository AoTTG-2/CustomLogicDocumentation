# Map
Inherits from object
## Methods
|Function|Returns|Description|
|---|---|---|
|FindAllMapObjects()|[List](../objects/list.md)|Find all map objects|
|FindMapObjectByName(objectName : [String](../static/string.md))|[MapObject](../objects/mapobject.md)|Find a map object by name|
|FindMapObjectsByName(objectName : [String](../static/string.md))|[List](../objects/list.md)|Find all map objects by name|
|FindMapObjectByComponent(className : [String](../static/string.md))|[MapObject](../objects/mapobject.md)|Find all map objects by component|
|FindMapObjectsByComponent(className : [String](../static/string.md))|[List](../objects/list.md)|Find all map objects by component|
|FindMapObjectByID(id : int)|[MapObject](../objects/mapobject.md)|Find a map object by ID|
|FindMapObjectByTag(tag : [String](../static/string.md))|[MapObject](../objects/mapobject.md)|Find a map object by tag|
|FindMapObjectsByTag(tag : [String](../static/string.md))|[List](../objects/list.md)|Find all map objects by tag|
|CreateMapObjectRaw(prefab : [String](../static/string.md))|[MapObject](../objects/mapobject.md)|Create a new map object|
|DestroyMapObject(mapObject : [MapObject](../objects/mapobject.md), includeChildren : bool)|none|Destroy a map object|
|CopyMapObject(mapObject : [MapObject](../objects/mapobject.md), includeChildren : bool)|[MapObject](../objects/mapobject.md)|Copy a map object|
|DestroyMapTargetable(targetable : [MapTargetable](../objects/maptargetable.md))|none|Destroy a map targetable|
|UpdateNavMesh()|none|Update the nav mesh|
|UpdateNavMeshAsync()|none|Update the nav mesh asynchronously|
