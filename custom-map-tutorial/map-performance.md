# Map Performance

## Possible Causes for Slow Loading

* Large number of objects being loaded at once will slow down all players. Large map scripts will slow down people connecting to your server as they have to download the map script text.
* Generation of a large or complicated NavMesh
  * NavMesh is generated automatically with bounds based on the set of all objects with physical colliders. Boundary size is currently capped within a 20kx20kx20k cube, this will likely change later when we swap to user defined navigation areas and pre-defined map boundaries.
  * Unity Terrain is complicated for navmesh generation due to the fact titans can ramp up the max slope allowed by unity's pathfinder. Spamming terrain for details without disabling the colliders will cause a massive slowdown.
  * Background objects outside your playable area with colliders enabled will add complexity to the navmesh. Please disable the colliders for these objects as it will save loading time.

## Possible Causes for Low Framerates

* Large number of non-static or unique objects
  * We use static batching in custom maps to reduce the number of drawcalls by batching together static objects which use the same mesh and material. Marking objects as not static will let said objects be moved and altered but will increase the number of drawcalls. If a map maker decides to spawn in 1 of each object in a map, marking them as static will also mean that essentially no batching is happening as the objects will all have separate mesh/materials.
* Large number of light sources
  * Light sources (at least with the current renderer) are somewhat expensive. Please try to limit the density of point lights so that they can be more efficiently distance culled.
    * Ex: If a lamppost has 4 lamps on it, please only actually use 1 light source to light up the area.
* Large number of colliders
  * Colliders, and especially non-convex mesh colliders take up performance when they are in a scene. If an object does not need to handle collisions (ex: background objects), please disable the collider.
* Large number of particle systems/VFX
  * VFX are another somewhat costly feature. Some effects will be efficient while others might not be depending on the scale and density. These are also not being distance culled (yet) and so depending on how many you want to use, you may need to implement distance culling via a custom component or game logic. (On Init, cache all vfx objects in a list and cull based on distance OnTick, if this is slow, you may need to implement a more complicated solution using quadtrees or just wait until we add it)
* Large number of rigidbody objects
  * Rigidbodies are simulated by the physics engine and are costly, marking them as networked also adds some overhead so limit the number of these objects.

