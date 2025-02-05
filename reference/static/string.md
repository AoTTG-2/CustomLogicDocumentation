# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/string.md)|False|Returns the newline character.|
## Methods
|Function|Returns|Description|
|---|---|---|
|FormatFloat(val : float, decimals : int)|[String](../static/string.md)|Formats a float to a string with the specified number of decimal places.|
|FormatFromList(str : [String](../static/string.md), list : [List](../objects/list.md))|[String](../static/string.md)|Equivalent to C# string.format(string, List<string>).|
|Split(toSplit : [String](../static/string.md), splitter : Object, removeEmptyEntries : bool = False)|[List](../objects/list.md)|Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.|
|Join(list : [List](../objects/list.md), separator : [String](../static/string.md))|[String](../static/string.md)|Joins a list of strings into a single string with the specified separator.|
|Substring(str : [String](../static/string.md), startIndex : int)|[String](../static/string.md)|Returns a substring starting from the specified index.|
|SubstringWithLength(str : [String](../static/string.md), startIndex : int, length : int)|[String](../static/string.md)|Returns a substring of the specified length starting from the specified start index.|
|Length(str : [String](../static/string.md))|int|Length of the string.|
|Replace(str : [String](../static/string.md), replace : [String](../static/string.md), with : [String](../static/string.md))|[String](../static/string.md)|Replaces all occurrences of a substring with another substring.|
|Contains(str : [String](../static/string.md), match : [String](../static/string.md))|bool|Checks if the string contains the specified substring.|
|StartsWith(str : [String](../static/string.md), match : [String](../static/string.md))|bool|Checks if the string starts with the specified substring.|
|EndsWith(str : [String](../static/string.md), match : [String](../static/string.md))|bool|Checks if the string ends with the specified substring.|
|Trim(str : [String](../static/string.md))|[String](../static/string.md)|Trims whitespace from the start and end of the string.|
|Insert(str : [String](../static/string.md), insert : [String](../static/string.md), index : int)|[String](../static/string.md)|Inserts a substring at the specified index.|
|Capitalize(str : [String](../static/string.md))|[String](../static/string.md)|Capitalizes the first letter of the string.|
|ToUpper(str : [String](../static/string.md))|[String](../static/string.md)|Converts the string to uppercase.|
|ToLower(str : [String](../static/string.md))|[String](../static/string.md)|Converts the string to lowercase.|
|IndexOf(str : [String](../static/string.md), substring : [String](../static/string.md))|int|Returns the index of the given string.|
