# Quaternion

Inherits from Object. Is a struct, meaning that assignments will create copies and comparisons will return true if all fields are equivalent.

### Initialization

Quaternion takes four floats X, Y, Z and W as parameters when initializing. \
Example: `quaternion = Quaternion(0.5, 0.5, 0.5, 0.5);`

### Fields

<table><thead><tr><th width="175.33333333333331">Field</th><th width="99">Type</th><th width="103">Readonly</th><th>Description</th></tr></thead><tbody><tr><td>X</td><td>float</td><td>false</td><td>X value of the quaternion.</td></tr><tr><td>Y</td><td>float</td><td>false</td><td>Y value of the quaternion.</td></tr><tr><td>Z</td><td>float</td><td>false</td><td>Z value of the quaternion.</td></tr><tr><td>W</td><td>float</td><td>false</td><td>W value of the quaternion.</td></tr><tr><td>Euler</td><td>Vector3</td><td>true</td><td>Returns the euler angles of the quaternion as a Vector3.</td></tr></tbody></table>

### Static Fields

Can be accessed by referencing Quaternion directly (example: Quaternion.Identity)

| Field    | Type       | Description                                |
| -------- | ---------- | ------------------------------------------ |
| Identity | Quaternion | Returns the identity quaternion (0,0,0,0). |

### Static functions

<table><thead><tr><th width="233.33333333333331">Function</th><th width="149">Returns</th><th>Description</th></tr></thead><tbody><tr><td>Lerp(a: Quaternion, b: Quaternion, t: float)</td><td>Quaternion</td><td>Returns a Quaternion lerped between a and b using scale t. T must be between 0 and 1.</td></tr><tr><td>LerpUnclamped(a: Quaternion, b: Quaternion, t: float)</td><td>Quaternion</td><td>Returns a Quaternion lerped between a and b using scale t. T can be outside 0 and 1.</td></tr><tr><td>Slerp(a: Quaternion, b: Quaternion, t: float)</td><td>Quaternion</td><td>Returns a Quaternion spherical lerped between a and b using scale t. T must be between 0 and 1.</td></tr><tr><td>SlerpUnclamped(a: Quaternion, b: Quaternion, t: float)</td><td>Quaternion</td><td>Returns a Quaternion spherical lserped between a and b using scale t. T can be outside 0 and 1.</td></tr><tr><td>FromEuler(v: Vector3)</td><td>Quaternion</td><td>Returns the Quaternion rotation from the given euler angles.</td></tr><tr><td>LookRotation(forward: Vector3, [optional] up: Vector3)</td><td>Quaternion</td><td>Returns the Quaternion rotation with the specified forward and (optional) up Vector.</td></tr><tr><td>FromToRotation(from: Vector3, to: Vector3)</td><td>Quaternion</td><td>Returns the Quaternion rotation between the from and to Vector.</td></tr><tr><td>Inverse(a: Quaternion)</td><td>Quaternion</td><td>Returns the inverse of the given Quaternion.</td></tr><tr><td>RotateTowards(from: Quaternion, to: Quaternion, maxDegrees: float)</td><td>Quaternion</td><td>Returns the quaternion rotated towards To with a maximum degree change.</td></tr></tbody></table>
