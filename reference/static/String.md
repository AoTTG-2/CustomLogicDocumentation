# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">FormatFloat</mark>(<mark style="color:blue;">float</mark> <mark style="color:yellow;">val</mark>, <mark style="color:blue;">int</mark> <mark style="color:yellow;">decimals</mark>)
Formats a float to a string with the specified number of decimal places.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">FormatFromList</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>, <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">list</mark>)
Equivalent to C# string.format(string, List<string>).
#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">Split</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">toSplit</mark>, <mark style="color:blue;">Object</mark> <mark style="color:yellow;">splitter</mark>, <mark style="color:blue;">bool</mark> <mark style="color:yellow;">removeEmptyEntries</mark> = <mark style="color:blue;">False</mark>)
Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Join</mark>(<mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">list</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">separator</mark>)
Joins a list of strings into a single string with the specified separator.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Substring</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>, <mark style="color:blue;">int</mark> <mark style="color:yellow;">startIndex</mark>)
Returns a substring starting from the specified index.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">SubstringWithLength</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>, <mark style="color:blue;">int</mark> <mark style="color:yellow;">startIndex</mark>, <mark style="color:blue;">int</mark> <mark style="color:yellow;">length</mark>)
Returns a substring of the specified length starting from the specified start index.
#### <mark style="color:blue;">int</mark> <mark style="color:yellow;">Length</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>)
Length of the string.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Replace</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">replace</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">with</mark>)
Replaces all occurrences of a substring with another substring.
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">Contains</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">match</mark>)
Checks if the string contains the specified substring.
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">StartsWith</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">match</mark>)
Checks if the string starts with the specified substring.
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">EndsWith</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">match</mark>)
Checks if the string ends with the specified substring.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Trim</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>)
Trims whitespace from the start and end of the string.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Insert</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">insert</mark>, <mark style="color:blue;">int</mark> <mark style="color:yellow;">index</mark>)
Inserts a substring at the specified index.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Capitalize</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>)
Capitalizes the first letter of the string.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">ToUpper</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>)
Converts the string to uppercase.
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">ToLower</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>)
Converts the string to lowercase.
#### <mark style="color:blue;">int</mark> <mark style="color:yellow;">IndexOf</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">str</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">substring</mark>)
Returns the index of the given string.

---

