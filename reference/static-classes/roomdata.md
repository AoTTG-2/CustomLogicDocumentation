# RoomData

Store and retrieve room variables. Room data is cleared upon joining or creating a new lobby and does not reset between game rounds. Supports float, string, bool, and int types.

Note that RoomData is local only and does not sync. You must use network messages to sync room variables.

<table><thead><tr><th width="271">Function</th><th width="101.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>SetProperty(name: string, value: object)</td><td>null</td><td>Sets the property with given name to the object value. Valid value types are float, string, bool, and int.</td></tr><tr><td>GetProperty(name: string, defaultValue: object)</td><td>object</td><td>Gets the property with given name. If property does not exist, returns defaultValue.</td></tr><tr><td>Clear()</td><td>null</td><td>Clears all room data.</td></tr></tbody></table>
