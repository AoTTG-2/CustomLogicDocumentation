# Json

Serializes and deserializes primitive and struct values from and to json strings. Supports float, int, string, bool, Vector3, Quaternion, Color, Dict, and List. Dict and List must contain only the supported types, and can be nested.

<table><thead><tr><th width="271">Function</th><th width="101.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>LoadFromString(value: string)</td><td>object</td><td>Deserializes the object from a json string.</td></tr><tr><td>SaveToString(value: object)</td><td>string</td><td>Serializes the object to a json string.</td></tr></tbody></table>
