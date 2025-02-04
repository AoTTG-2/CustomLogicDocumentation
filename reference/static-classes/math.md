# Math

Math functions. Note that parameter types can be either int or float unless otherwise specified. Functions may return int or float depending on the parameter types given.

### Fields



| Field           | Type  | Readonly | Description    |
| --------------- | ----- | -------- | -------------- |
| PI              | float | true     | Mathf.PI       |
| Infinity        | float | true     | Mathf.Infinity |
| Rad2DegConstant | float | true     | Mathf.Rad2Deg  |
| Deg2RadConstant | float | true     | Mathf.Deg2Rad  |

### Functions

<table><thead><tr><th width="235">Function</th><th width="160.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>Clamp(value, min, max)</td><td>int/float</td><td>Clamps the value between min and max.</td></tr><tr><td>Max(a, b)</td><td>int/float</td><td>Maximum of a and b.</td></tr><tr><td>Min(a, b)</td><td>int/float</td><td>Minimum of a and b.</td></tr><tr><td>Pow(a, b)</td><td>float</td><td>a to the power of b.</td></tr><tr><td>Abs(a)</td><td>int/float</td><td>Absolute value of a.</td></tr><tr><td>Sqrt(a)</td><td>float</td><td>Square root of a.</td></tr><tr><td>Mod(a, b)</td><td>int</td><td>Modulo of a % b</td></tr><tr><td>Ceil(a)</td><td>int</td><td>Rounds to higher int.</td></tr><tr><td>Floor(a)</td><td>int</td><td>Rounds to lower int.</td></tr><tr><td>Round(a)</td><td>int</td><td>Rounds to nearest int.</td></tr><tr><td>Sin(a)</td><td>float</td><td>Sin of a, in degrees.</td></tr><tr><td>Cos(a)</td><td>float</td><td>Cosine of a.</td></tr><tr><td>Tan(a)</td><td>float</td><td>Tan of a.</td></tr><tr><td>Asin(a)</td><td>float</td><td>Arcsin of a, in degrees.</td></tr><tr><td>Acos(a)</td><td>float</td><td>Arccos of a.</td></tr><tr><td>Atan(a)</td><td>float</td><td>Arctan of a.</td></tr><tr><td>Atan2(a, b)</td><td>float</td><td>Atan2 of a and b.</td></tr><tr><td>Deg2Rad(a)</td><td>float</td><td>Converts a degrees to radians.</td></tr><tr><td>Rad2Deg(a)</td><td>float</td><td>Converts a radians to degrees.</td></tr><tr><td>Lerp(a, b, t)</td><td>float</td><td>Linearly interpolates between <code>a</code> and <code>b</code> by <code>t</code> where <code>t</code> is limited from 0 to 1.</td></tr><tr><td>LerpUnclamped(a, b, t)</td><td>float</td><td>Linearly interpolates between <code>a</code> and <code>b</code> by <code>t</code> with no limit to <code>t</code>.</td></tr><tr><td>Sign(a)</td><td>float</td><td>Returns a value of 1 when <code>a</code> is 0 or greater. Returns a value of -1 when <code>a</code> is negative.</td></tr></tbody></table>

