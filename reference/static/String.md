# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">FormatFloat</span>(<span style="color:blue;">float</span> val, <span style="color:blue;">int</span> decimals)
> Formats a float to a string with the specified number of decimal places.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">FormatFromList</span>(<span style="color:blue;">[String](../static/String.md)</span> str, <span style="color:blue;">[List](../objects/List.md)</span> list)
> Equivalent to C# string.format(string, List<string>).
#### <span style="color:blue;">[List](../objects/List.md)</span> <span style="color:yellow;">Split</span>(<span style="color:blue;">[String](../static/String.md)</span> toSplit, <span style="color:blue;">Object</span> splitter, <span style="color:blue;">bool</span> removeEmptyEntries = <span style="color:blue;">False</span>)
> Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">Join</span>(<span style="color:blue;">[List](../objects/List.md)</span> list, <span style="color:blue;">[String](../static/String.md)</span> separator)
> Joins a list of strings into a single string with the specified separator.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">Substring</span>(<span style="color:blue;">[String](../static/String.md)</span> str, <span style="color:blue;">int</span> startIndex)
> Returns a substring starting from the specified index.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">SubstringWithLength</span>(<span style="color:blue;">[String](../static/String.md)</span> str, <span style="color:blue;">int</span> startIndex, <span style="color:blue;">int</span> length)
> Returns a substring of the specified length starting from the specified start index.
#### <span style="color:blue;">int</span> <span style="color:yellow;">Length</span>(<span style="color:blue;">[String](../static/String.md)</span> str)
> Length of the string.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">Replace</span>(<span style="color:blue;">[String](../static/String.md)</span> str, <span style="color:blue;">[String](../static/String.md)</span> replace, <span style="color:blue;">[String](../static/String.md)</span> with)
> Replaces all occurrences of a substring with another substring.
#### <span style="color:blue;">bool</span> <span style="color:yellow;">Contains</span>(<span style="color:blue;">[String](../static/String.md)</span> str, <span style="color:blue;">[String](../static/String.md)</span> match)
> Checks if the string contains the specified substring.
#### <span style="color:blue;">bool</span> <span style="color:yellow;">StartsWith</span>(<span style="color:blue;">[String](../static/String.md)</span> str, <span style="color:blue;">[String](../static/String.md)</span> match)
> Checks if the string starts with the specified substring.
#### <span style="color:blue;">bool</span> <span style="color:yellow;">EndsWith</span>(<span style="color:blue;">[String](../static/String.md)</span> str, <span style="color:blue;">[String](../static/String.md)</span> match)
> Checks if the string ends with the specified substring.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">Trim</span>(<span style="color:blue;">[String](../static/String.md)</span> str)
> Trims whitespace from the start and end of the string.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">Insert</span>(<span style="color:blue;">[String](../static/String.md)</span> str, <span style="color:blue;">[String](../static/String.md)</span> insert, <span style="color:blue;">int</span> index)
> Inserts a substring at the specified index.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">Capitalize</span>(<span style="color:blue;">[String](../static/String.md)</span> str)
> Capitalizes the first letter of the string.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">ToUpper</span>(<span style="color:blue;">[String](../static/String.md)</span> str)
> Converts the string to uppercase.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">ToLower</span>(<span style="color:blue;">[String](../static/String.md)</span> str)
> Converts the string to lowercase.
#### <span style="color:blue;">int</span> <span style="color:yellow;">IndexOf</span>(<span style="color:blue;">[String](../static/String.md)</span> str, <span style="color:blue;">[String](../static/String.md)</span> substring)
> Returns the index of the given string.

---

