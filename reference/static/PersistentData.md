# PersistentData
Inherits from object
## Static Methods
|Function|Returns|Description|
|---|---|---|
|SetProperty(<br/><i>property</i> : [String](../static/String.md),<br/><i>value</i> : Object<br/>)|none|Sets the property with given name to the object value. Valid value types are float, string, bool, and int.|
|GetProperty(<br/><i>property</i> : [String](../static/String.md),<br/><i>defaultValue</i> : Object<br/>)|Object|Gets the property with given name. If property does not exist, returns defaultValue.|
|LoadFromFile(<br/><i>fileName</i> : [String](../static/String.md),<br/><i>encrypted</i> : bool<br/>)|none|Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.|
|SaveToFile(<br/><i>fileName</i> : [String](../static/String.md),<br/><i>encrypted</i> : bool<br/>)|none|Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.|
|Clear()|none|Clears current persistent data.|
|IsValidFileName(<i>fileName</i> : [String](../static/String.md))|bool|Determines whether or not the given fileName will be allowed for use when saving/loading a file.|
|FileExists(<i>fileName</i> : [String](../static/String.md))|bool|Determines whether the file given already exists. Throws an error if given an invalid file name.|
