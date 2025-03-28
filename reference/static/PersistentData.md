# PersistentData
Inherits from object
## Static Methods
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SetProperty</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">property</span>, <span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">value</span>)
Sets the property with given name to the object value. Valid value types are float, string, bool, and int.
#### <span style="color:#509cd4">Object</span> <span style="color:#dcdcaa">GetProperty</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">property</span>, <span style="color:#509cd4">Object</span> <span style="color:#9cdcfe">defaultValue</span>)
Gets the property with given name. If property does not exist, returns defaultValue.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">LoadFromFile</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">fileName</span>, <span style="color:#509cd4">bool</span> <span style="color:#9cdcfe">encrypted</span>)
Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SaveToFile</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">fileName</span>, <span style="color:#509cd4">bool</span> <span style="color:#9cdcfe">encrypted</span>)
Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Clear</span>()
Clears current persistent data.
#### <span style="color:#509cd4">bool</span> <span style="color:#dcdcaa">IsValidFileName</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">fileName</span>)
Determines whether or not the given fileName will be allowed for use when saving/loading a file.
#### <span style="color:#509cd4">bool</span> <span style="color:#dcdcaa">FileExists</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">fileName</span>)
Determines whether the file given already exists. Throws an error if given an invalid file name.

---

