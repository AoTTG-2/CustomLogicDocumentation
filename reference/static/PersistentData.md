# PersistentData
Inherits from object
## Static Methods
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetProperty</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">property</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">value</mark>)
Sets the property with given name to the object value. Valid value types are float, string, bool, and int.
#### <mark style="color:#509cd4;">Object</mark> <mark style="color:#dcdcaa;">GetProperty</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">property</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">defaultValue</mark>)
Gets the property with given name. If property does not exist, returns defaultValue.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">LoadFromFile</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">fileName</mark>, <mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">encrypted</mark>)
Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SaveToFile</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">fileName</mark>, <mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">encrypted</mark>)
Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Clear</mark>()
Clears current persistent data.
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">IsValidFileName</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">fileName</mark>)
Determines whether or not the given fileName will be allowed for use when saving/loading a file.
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">FileExists</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">fileName</mark>)
Determines whether the file given already exists. Throws an error if given an invalid file name.

---

