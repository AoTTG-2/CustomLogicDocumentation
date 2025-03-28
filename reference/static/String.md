# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">FormatFloat</mark>(<mark style="color:Blue;">float</mark> <mark style="color:Yellow;">val</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">decimals</mark>)
Formats a float to a string with the specified number of decimal places.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">FormatFromList</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>, <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">list</mark>)
Equivalent to C# string.format(string, List<string>).
#### <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">Split</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">toSplit</mark>, <mark style="color:Blue;">Object</mark> <mark style="color:Yellow;">splitter</mark>, <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">removeEmptyEntries</mark> = <mark style="color:Blue;">False</mark>)
Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">Join</mark>(<mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">list</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">separator</mark>)
Joins a list of strings into a single string with the specified separator.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">Substring</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">startIndex</mark>)
Returns a substring starting from the specified index.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">SubstringWithLength</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">startIndex</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">length</mark>)
Returns a substring of the specified length starting from the specified start index.
#### <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">Length</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>)
Length of the string.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">Replace</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">replace</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">with</mark>)
Replaces all occurrences of a substring with another substring.
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">Contains</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">match</mark>)
Checks if the string contains the specified substring.
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">StartsWith</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">match</mark>)
Checks if the string starts with the specified substring.
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">EndsWith</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">match</mark>)
Checks if the string ends with the specified substring.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">Trim</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>)
Trims whitespace from the start and end of the string.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">Insert</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">insert</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">index</mark>)
Inserts a substring at the specified index.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">Capitalize</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>)
Capitalizes the first letter of the string.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">ToUpper</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>)
Converts the string to uppercase.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">ToLower</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>)
Converts the string to lowercase.
#### <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">IndexOf</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">str</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">substring</mark>)
Returns the index of the given string.

---

