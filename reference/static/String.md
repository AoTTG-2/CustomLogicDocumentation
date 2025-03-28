# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">FormatFloat</span>(<span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">val</span>, <span style="color:#509cd4;">int</span> <span style="color:#9cdcfe;">decimals</span>)
Formats a float to a string with the specified number of decimal places.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">FormatFromList</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>, <span style="color:#509cd4;">[List](../objects/List.md)</span> <span style="color:#9cdcfe;">list</span>)
Equivalent to C# string.format(string, List<string>).
#### <span style="color:#509cd4;">[List](../objects/List.md)</span> <span style="color:#dcdcaa;">Split</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">toSplit</span>, <span style="color:#509cd4;">Object</span> <span style="color:#9cdcfe;">splitter</span>, <span style="color:#509cd4;">bool</span> <span style="color:#9cdcfe;">removeEmptyEntries</span> = <span style="color:#509cd4;">False</span>)
Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">Join</span>(<span style="color:#509cd4;">[List](../objects/List.md)</span> <span style="color:#9cdcfe;">list</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">separator</span>)
Joins a list of strings into a single string with the specified separator.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">Substring</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>, <span style="color:#509cd4;">int</span> <span style="color:#9cdcfe;">startIndex</span>)
Returns a substring starting from the specified index.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">SubstringWithLength</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>, <span style="color:#509cd4;">int</span> <span style="color:#9cdcfe;">startIndex</span>, <span style="color:#509cd4;">int</span> <span style="color:#9cdcfe;">length</span>)
Returns a substring of the specified length starting from the specified start index.
#### <span style="color:#509cd4;">int</span> <span style="color:#dcdcaa;">Length</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>)
Length of the string.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">Replace</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">replace</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">with</span>)
Replaces all occurrences of a substring with another substring.
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">Contains</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">match</span>)
Checks if the string contains the specified substring.
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">StartsWith</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">match</span>)
Checks if the string starts with the specified substring.
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">EndsWith</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">match</span>)
Checks if the string ends with the specified substring.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">Trim</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>)
Trims whitespace from the start and end of the string.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">Insert</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">insert</span>, <span style="color:#509cd4;">int</span> <span style="color:#9cdcfe;">index</span>)
Inserts a substring at the specified index.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">Capitalize</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>)
Capitalizes the first letter of the string.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">ToUpper</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>)
Converts the string to uppercase.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">ToLower</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>)
Converts the string to lowercase.
#### <span style="color:#509cd4;">int</span> <span style="color:#dcdcaa;">IndexOf</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">str</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">substring</span>)
Returns the index of the given string.

---

