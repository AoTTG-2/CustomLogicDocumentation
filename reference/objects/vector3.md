# Vector3

Inherits from Object. Is a struct, meaning that assignments will create copies and comparisons will return true if all fields are equivalent.

### Initialization

Vector3 takes up to three floats X, Y, and Z as parameters when initializing.&#x20;

```python
# create an empty 0,0,0 vector
vector = Vector3();

# create a vector with x=5.5, y=6.0, z=24.8
vector = Vector3(5.5, 6.0, 24.8);

# create a vector with x,y,z = 1.2
vector = Vector3(1.2);

# create a vector with x=5.5, y=6.0, z=0
vector = Vector3(5.5, 6.0);
```

### Fields

<table><thead><tr><th width="175.33333333333331">Field</th><th width="99">Type</th><th width="103">Readonly</th><th>Description</th></tr></thead><tbody><tr><td>X</td><td>float</td><td>false</td><td>X axis of the vector.</td></tr><tr><td>Y</td><td>float</td><td>false</td><td>Y axis of the vector.</td></tr><tr><td>Z</td><td>float</td><td>false</td><td>Z axis of the vector.</td></tr><tr><td>Normalized</td><td>Vector3</td><td>true</td><td>Normalized version of the vector.</td></tr><tr><td>Magnitude</td><td>float</td><td>true</td><td>Returns the magnitude of the vector.</td></tr></tbody></table>

### Functions

<table><thead><tr><th width="249">Function</th><th width="153.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>Scale(scale: float)</td><td>Vector3</td><td>Returns the Vector3 multiplied by scale.</td></tr></tbody></table>

### Static Fields

Can be accessed by referencing Vector3 directly (example: Vector3.Up)

| Field   | Type    | Description |
| ------- | ------- | ----------- |
| Up      | Vector3 |             |
| Down    | Vector3 |             |
| Left    | Vector3 |             |
| Right   | Vector3 |             |
| Forward | Vector3 |             |
| Back    | Vector3 |             |
| Zero    | Vector3 |             |
| One     | Vector3 |             |

### Static functions

<table><thead><tr><th width="233.33333333333331">Function</th><th width="149">Returns</th><th>Description</th></tr></thead><tbody><tr><td>Lerp(a: Vector3, b: Vector3, t: float)</td><td>Vector3</td><td>Returns a Vector3 lerped between a and b using scale t. T must be between 0 and 1.</td></tr><tr><td>LerpUnclamped(a: Vector3, b: Vector3, t: float)</td><td>Vector3</td><td>Returns a Vector3 lerped between a and b using scale t. T can be outside 0 and 1.</td></tr><tr><td>Slerp(a: Vector3, b: Vector3, t: float)</td><td>Vector3</td><td>Returns a Vector3 spherical lerped between a and b using scale t. T must be between 0 and 1.</td></tr><tr><td>SlerpUnclamped(a: Vector3, b: Vector3, t: float)</td><td>Vector3</td><td>Returns a Vector3 spherical lerped between a and b using scale t. T can be outside 0 and 1.</td></tr><tr><td>GetRotationDirection(a: Vector3, b: Vector3)</td><td>Vector3</td><td>Gets the relational Vector3 b using a as a reference. This is equivalent to setting MapObject.Forward to Vector a, and finding the relative b vector.</td></tr><tr><td>Distance(a: Vector3, b: Vector3)</td><td>float</td><td>Returns the distance between two Vector3s.</td></tr><tr><td>Project(a: Vector3, b: Vector3)</td><td>Vector3</td><td>Returns a projected on b.</td></tr><tr><td>Multiply(a: Vector3, b: Vector3)</td><td>Vector3</td><td>Returns the Vector3 of each element in a multiplied by each element of b. It returns the Vector3(a.X * b.X, a.Y * b.Y, a.Z * b.Z).</td></tr><tr><td>Divide(a: Vector3, b: Vector3)</td><td>Vector3</td><td>Returns the Vector3 of each element in a divided by each element of b.</td></tr><tr><td>Angle(a: Vector3, b: Vector3)</td><td>float</td><td>Returns the angle between a and b. Always a positive value.</td></tr><tr><td>SignedAngle(a: Vector3, b: Vector3, axis: Vector3)</td><td>float</td><td>Returns the signed angle between a and b using the given axis.</td></tr><tr><td>Cross(a: Vector3, b: Vector3)</td><td>Vector</td><td>Returns the cross product of a and b.</td></tr><tr><td>Dot(a: Vector3, b: Vector3)</td><td>float</td><td>Returns the dot product of a and b.</td></tr><tr><td>RotateTowards(a: Vector3, b: Vector3, maxAngle: float, maxMagnitude: float)</td><td>Vector3</td><td>Returns the Vector3 that is rotated from a to b using maxAngle degrees and changing magnitude by at most maxMagnitude.</td></tr></tbody></table>
