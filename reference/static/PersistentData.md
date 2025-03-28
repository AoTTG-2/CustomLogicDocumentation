# PersistentData
Inherits from object
## Static Methods
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetProperty</span>(<span style="color:blue;">[String](../static/String.md)</span> property, <span style="color:blue;">Object</span> value)
> Sets the property with given name to the object value. Valid value types are float, string, bool, and int.
#### <span style="color:blue;">Object</span> <span style="color:yellow;">GetProperty</span>(<span style="color:blue;">[String](../static/String.md)</span> property, <span style="color:blue;">Object</span> defaultValue)
> Gets the property with given name. If property does not exist, returns defaultValue.
#### <span style="color:blue;">void</span> <span style="color:yellow;">LoadFromFile</span>(<span style="color:blue;">[String](../static/String.md)</span> fileName, <span style="color:blue;">bool</span> encrypted)
> Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SaveToFile</span>(<span style="color:blue;">[String](../static/String.md)</span> fileName, <span style="color:blue;">bool</span> encrypted)
> Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.
#### <span style="color:blue;">void</span> <span style="color:yellow;">Clear</span>()
> Clears current persistent data.
#### <span style="color:blue;">bool</span> <span style="color:yellow;">IsValidFileName</span>(<span style="color:blue;">[String](../static/String.md)</span> fileName)
> Determines whether or not the given fileName will be allowed for use when saving/loading a file.
#### <span style="color:blue;">bool</span> <span style="color:yellow;">FileExists</span>(<span style="color:blue;">[String](../static/String.md)</span> fileName)
> Determines whether the file given already exists. Throws an error if given an invalid file name.

---

