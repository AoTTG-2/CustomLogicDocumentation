# MapTargetable

MapTargetable object returned from MapObject.AddTarget method.&#x20;

Creating a map targetable is similar to adding a collider to the MapObject, except this collider can be targeted by AI such as titans. Map targetables that are on a different team than the AI will be targeted by the titan, and will trigger the OnGetHit callback on the attached MapObject.



| Fields   | Type    | Readonly | Description                                   |
| -------- | ------- | -------- | --------------------------------------------- |
| Team     | string  | false    | Team map targetable belongs to.               |
| Enabled  | bool    | false    | Whether the map targetable is enabled or not. |
| Position | Vector3 | true     | World position of the map targetable.         |
