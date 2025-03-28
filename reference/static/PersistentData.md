# PersistentData
Inherits from object
## Static Methods
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetProperty</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">property</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">value</mark>)
Sets the property with given name to the object value. Valid value types are float, string, bool, and int.
#### <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">GetProperty</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">property</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">defaultValue</mark>)
Gets the property with given name. If property does not exist, returns defaultValue.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">LoadFromFile</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">fileName</mark>, <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">encrypted</mark>)
Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SaveToFile</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">fileName</mark>, <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">encrypted</mark>)
Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Clear</mark>()
Clears current persistent data.
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">IsValidFileName</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">fileName</mark>)
Determines whether or not the given fileName will be allowed for use when saving/loading a file.
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">FileExists</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">fileName</mark>)
Determines whether the file given already exists. Throws an error if given an invalid file name.

---

