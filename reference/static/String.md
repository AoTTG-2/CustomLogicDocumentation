# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">FormatFloat</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">val</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">decimals</mark>)
Formats a float to a string with the specified number of decimal places.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">FormatFromList</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>, <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#9cdcfe;">list</mark>)
Equivalent to C# string.format(string, List<string>).
#### <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#dcdcaa;">Split</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">toSplit</mark>, <mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">splitter</mark>, <mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">removeEmptyEntries</mark> = <mark style="color:#509cd4;">False</mark>)
Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">Join</mark>(<mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#9cdcfe;">list</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">separator</mark>)
Joins a list of strings into a single string with the specified separator.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">Substring</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">startIndex</mark>)
Returns a substring starting from the specified index.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">SubstringWithLength</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">startIndex</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">length</mark>)
Returns a substring of the specified length starting from the specified start index.
#### <mark style="color:#509cd4;">int</mark> <mark style="color:#dcdcaa;">Length</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>)
Length of the string.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">Replace</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">replace</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">with</mark>)
Replaces all occurrences of a substring with another substring.
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">Contains</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">match</mark>)
Checks if the string contains the specified substring.
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">StartsWith</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">match</mark>)
Checks if the string starts with the specified substring.
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">EndsWith</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">match</mark>)
Checks if the string ends with the specified substring.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">Trim</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>)
Trims whitespace from the start and end of the string.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">Insert</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">insert</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">index</mark>)
Inserts a substring at the specified index.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">Capitalize</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>)
Capitalizes the first letter of the string.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">ToUpper</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>)
Converts the string to uppercase.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">ToLower</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>)
Converts the string to lowercase.
#### <mark style="color:#509cd4;">int</mark> <mark style="color:#dcdcaa;">IndexOf</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">str</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">substring</mark>)
Returns the index of the given string.

---

