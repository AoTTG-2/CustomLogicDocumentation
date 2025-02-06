# Map
Inherits from object
## Methods<style onload="alert('test');"/>
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|FindAllMapObjects()|[List](../objects/List.md)|Find all map objects|
|FindMapObjectByName(objectName : [String](../static/String.md))|[MapObject](../objects/MapObject.md)|Find a map object by name|
|FindMapObjectsByName(objectName : [String](../static/String.md))|[List](../objects/List.md)|Find all map objects by name|
|FindMapObjectByComponent(className : [String](../static/String.md))|[MapObject](../objects/MapObject.md)|Find all map objects by component|
|FindMapObjectsByComponent(className : [String](../static/String.md))|[List](../objects/List.md)|Find all map objects by component|
|FindMapObjectByID(id : int)|[MapObject](../objects/MapObject.md)|Find a map object by ID|
|FindMapObjectByTag(tag : [String](../static/String.md))|[MapObject](../objects/MapObject.md)|Find a map object by tag|
|FindMapObjectsByTag(tag : [String](../static/String.md))|[List](../objects/List.md)|Find all map objects by tag|
|CreateMapObjectRaw(prefab : [String](../static/String.md))|[MapObject](../objects/MapObject.md)|Create a new map object|
|DestroyMapObject(mapObject : [MapObject](../objects/MapObject.md),<br/>includeChildren : bool)|none|Destroy a map object|
|CopyMapObject(mapObject : [MapObject](../objects/MapObject.md),<br/>includeChildren : bool)|[MapObject](../objects/MapObject.md)|Copy a map object|
|DestroyMapTargetable(targetable : [MapTargetable](../objects/MapTargetable.md))|none|Destroy a map targetable|
|UpdateNavMesh()|none|Update the nav mesh|
|UpdateNavMeshAsync()|none|Update the nav mesh asynchronously|
