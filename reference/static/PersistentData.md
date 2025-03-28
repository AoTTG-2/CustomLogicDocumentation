# PersistentData
Inherits from object
## Static Methods
#### void <span style="color":#dcdcaa>SetProperty<span>([String](../static/String.md) <span style="color":#9cdcfe>property<span>, Object <span style="color":#9cdcfe>value<span>)
Sets the property with given name to the object value. Valid value types are float, string, bool, and int.
#### Object <span style="color":#dcdcaa>GetProperty<span>([String](../static/String.md) <span style="color":#9cdcfe>property<span>, Object <span style="color":#9cdcfe>defaultValue<span>)
Gets the property with given name. If property does not exist, returns defaultValue.
#### void <span style="color":#dcdcaa>LoadFromFile<span>([String](../static/String.md) <span style="color":#9cdcfe>fileName<span>, bool <span style="color":#9cdcfe>encrypted<span>)
Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.
#### void <span style="color":#dcdcaa>SaveToFile<span>([String](../static/String.md) <span style="color":#9cdcfe>fileName<span>, bool <span style="color":#9cdcfe>encrypted<span>)
Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.
#### void <span style="color":#dcdcaa>Clear<span>()
Clears current persistent data.
#### bool <span style="color":#dcdcaa>IsValidFileName<span>([String](../static/String.md) <span style="color":#9cdcfe>fileName<span>)
Determines whether or not the given fileName will be allowed for use when saving/loading a file.
#### bool <span style="color":#dcdcaa>FileExists<span>([String](../static/String.md) <span style="color":#9cdcfe>fileName<span>)
Determines whether the file given already exists. Throws an error if given an invalid file name.

---

