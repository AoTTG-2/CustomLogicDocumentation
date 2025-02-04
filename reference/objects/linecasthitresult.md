# LineCastHitResult

Line cast hit result from Physics.LineCast.



| Fields      | Type    | Readonly | Description                                                 |
| ----------- | ------- | -------- | ----------------------------------------------------------- |
| IsCharacter | bool    | true     | Whether or not the LineCast hit a player                    |
| IsMapObject | bool    | true     | Whether or not the LineCast hit a MapObject                 |
| Point       | Vector3 | true     | The hit point.                                              |
| Normal      | Vector3 | true     | The normal vector of the face that was hit by the LineCast. |
| Distance    | float   | true     | The distance between the LineCast origin and the hit point. |
| Collider    | object  | true     | The collider hit by the LineCast.                           |
