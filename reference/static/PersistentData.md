# PersistentData
Inherits from object
## Static Methods
|Function|Returns|Description|
|---|---|---|
|SetProperty(property : [String](../static/String.md), value : Object)|none|Sets the property with given name to the object value. Valid value types are float, string, bool, and int.|
|GetProperty(property : [String](../static/String.md), defaultValue : Object)|Object|Gets the property with given name. If property does not exist, returns defaultValue.|
|LoadFromFile(fileName : [String](../static/String.md), encrypted : bool)|none|Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.|
|SaveToFile(fileName : [String](../static/String.md), encrypted : bool)|none|Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.|
|Clear()|none|Clears current persistent data.|
|IsValidFileName(fileName : [String](../static/String.md))|bool|Determines whether or not the given fileName will be allowed for use when saving/loading a file.|
|FileExists(fileName : [String](../static/String.md))|bool|Determines whether the file given already exists. Throws an error if given an invalid file name.|
