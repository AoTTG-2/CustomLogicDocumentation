# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">FormatFloat</mark>(<mark style="color:blue;">float</mark> val, <mark style="color:blue;">int</mark> decimals)
> Formats a float to a string with the specified number of decimal places.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">FormatFromList</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str, <mark style="color:blue;">[List](../objects/List.md)</mark> list)
> Equivalent to C# string.format(string, List<string>).

#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">Split</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> toSplit, <mark style="color:blue;">Object</mark> splitter, <mark style="color:blue;">bool</mark> removeEmptyEntries = <mark style="color:blue;">False</mark>)
> Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Join</mark>(<mark style="color:blue;">[List](../objects/List.md)</mark> list, <mark style="color:blue;">[String](../static/String.md)</mark> separator)
> Joins a list of strings into a single string with the specified separator.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Substring</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str, <mark style="color:blue;">int</mark> startIndex)
> Returns a substring starting from the specified index.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">SubstringWithLength</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str, <mark style="color:blue;">int</mark> startIndex, <mark style="color:blue;">int</mark> length)
> Returns a substring of the specified length starting from the specified start index.

#### <mark style="color:blue;">int</mark> <mark style="color:yellow;">Length</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str)
> Length of the string.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Replace</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str, <mark style="color:blue;">[String](../static/String.md)</mark> replace, <mark style="color:blue;">[String](../static/String.md)</mark> with)
> Replaces all occurrences of a substring with another substring.

#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">Contains</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str, <mark style="color:blue;">[String](../static/String.md)</mark> match)
> Checks if the string contains the specified substring.

#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">StartsWith</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str, <mark style="color:blue;">[String](../static/String.md)</mark> match)
> Checks if the string starts with the specified substring.

#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">EndsWith</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str, <mark style="color:blue;">[String](../static/String.md)</mark> match)
> Checks if the string ends with the specified substring.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Trim</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str)
> Trims whitespace from the start and end of the string.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Insert</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str, <mark style="color:blue;">[String](../static/String.md)</mark> insert, <mark style="color:blue;">int</mark> index)
> Inserts a substring at the specified index.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">Capitalize</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str)
> Capitalizes the first letter of the string.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">ToUpper</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str)
> Converts the string to uppercase.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">ToLower</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str)
> Converts the string to lowercase.

#### <mark style="color:blue;">int</mark> <mark style="color:yellow;">IndexOf</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> str, <mark style="color:blue;">[String](../static/String.md)</mark> substring)
> Returns the index of the given string.


---

