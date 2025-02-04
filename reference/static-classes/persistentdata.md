# PersistentData

Store and retrieve persistent data. Persistent data can be saved and loaded from file. Supports float, int, string, and bool types.

Note that any game mode may use the same file names, so it is recommended that you choose unique file names when saving and loading.

Saved files are located in Documents/Aottg2/PersistentData.

<table><thead><tr><th width="271">Function</th><th width="101.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>SetProperty(name: string, value: object)</td><td>null</td><td>Sets the property with given name to the object value. Valid value types are float, string, bool, and int.</td></tr><tr><td>GetProperty(name: string, defaultValue: object)</td><td>object</td><td>Gets the property with given name. If property does not exist, returns defaultValue.</td></tr><tr><td>Clear()</td><td>null</td><td>Clears current persistent data.</td></tr><tr><td>SaveToFile(fileName: string, encrypted: bool)</td><td>null</td><td>Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.</td></tr><tr><td>LoadFromFile(fileName: string, encrypted: bool)</td><td>null</td><td>Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.</td></tr><tr><td>IsValidFileName(fileName: string)</td><td>bool</td><td>Determines whether or not the given fileName will be allowed for use when saving/loading a file.</td></tr><tr><td>FileExists(fileName: string)</td><td>bool</td><td>Determines whether the file given already exists. Throws an error if given an invalid file name.</td></tr></tbody></table>

