# PersistentData
Inherits from object
## Static Methods
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetProperty</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> property, <mark style="color:blue;">Object</mark> value)
> Sets the property with given name to the object value. Valid value types are float, string, bool, and int.

#### <mark style="color:blue;">Object</mark> <mark style="color:yellow;">GetProperty</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> property, <mark style="color:blue;">Object</mark> defaultValue)
> Gets the property with given name. If property does not exist, returns defaultValue.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">LoadFromFile</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> fileName, <mark style="color:blue;">bool</mark> encrypted)
> Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SaveToFile</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> fileName, <mark style="color:blue;">bool</mark> encrypted)
> Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Clear</mark>()
> Clears current persistent data.

#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">IsValidFileName</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> fileName)
> Determines whether or not the given fileName will be allowed for use when saving/loading a file.

#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">FileExists</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> fileName)
> Determines whether the file given already exists. Throws an error if given an invalid file name.


---

