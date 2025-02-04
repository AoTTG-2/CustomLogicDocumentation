# NavMeshObstacle

Wraps the object in a NavMeshObstacle unity component auto-sized based on the collider sizes. If "Smart Movement" is enabled in Titan settings, titans will pathfind around obstacles unless trying to target a human which overrides navigation with aottg1's AI movement.

```
component NavMeshObstacle
{
    Description = "Adds a navMeshObstacle to the object";
    _nav = null;

    function Init()
    {
        # Add the component like how we add Rigidbody
        _nav = self.MapObject.AddBuiltinComponent("NavMeshObstacle", false);
    }
}
```
