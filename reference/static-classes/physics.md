# Physics

Some commonly used physics functions.

<table><thead><tr><th width="271">Function</th><th width="101.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>LineCast(start: Vector3, end: Vector3, collideWith: string)</td><td>LineCastHitResult</td><td>Performs a linecast between start and end vectors and colliding with the collideWith category (such as "Characters"). If an object is found return that object, otherwise return null.</td></tr><tr><td>SphereCast(start: Vector3, end: Vector3, radius: float, collideWith: string)</td><td>object</td><td>Performs a spherecast between start and end vectors with radius and colliding with the collideWith category (such as "Characters"). If an object is found return that object, otherwise return null.</td></tr></tbody></table>
