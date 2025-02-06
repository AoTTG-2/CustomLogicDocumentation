# Map
Inherits from object
## Methods
|Function|Returns|Description|
|---|---|---|
|FindAllMapObjects()|[List](../objects/List.md)|Find all map objects|
|FindMapObjectByName(<i>objectName</i> : [String](../static/String.md))|[MapObject](../objects/MapObject.md)|Find a map object by name|
|FindMapObjectsByName(<i>objectName</i> : [String](../static/String.md))|[List](../objects/List.md)|Find all map objects by name|
|FindMapObjectByComponent(<i>className</i> : [String](../static/String.md))|[MapObject](../objects/MapObject.md)|Find all map objects by component|
|FindMapObjectsByComponent(<i>className</i> : [String](../static/String.md))|[List](../objects/List.md)|Find all map objects by component|
|FindMapObjectByID(<i>id</i> : int)|[MapObject](../objects/MapObject.md)|Find a map object by ID|
|FindMapObjectByTag(<i>tag</i> : [String](../static/String.md))|[MapObject](../objects/MapObject.md)|Find a map object by tag|
|FindMapObjectsByTag(<i>tag</i> : [String](../static/String.md))|[List](../objects/List.md)|Find all map objects by tag|
|CreateMapObjectRaw(<i>prefab</i> : [String](../static/String.md))|[MapObject](../objects/MapObject.md)|Create a new map object|
|DestroyMapObject(<br/><i>mapObject</i> : [MapObject](../objects/MapObject.md),<br/><i>includeChildren</i> : bool<br/>)|none|Destroy a map object|
|CopyMapObject(<br/><i>mapObject</i> : [MapObject](../objects/MapObject.md),<br/><i>includeChildren</i> : bool<br/>)|[MapObject](../objects/MapObject.md)|Copy a map object|
|DestroyMapTargetable(<i>targetable</i> : [MapTargetable](../objects/MapTargetable.md))|none|Destroy a map targetable|
|UpdateNavMesh()|none|Update the nav mesh|
|UpdateNavMeshAsync()|none|Update the nav mesh asynchronously|
