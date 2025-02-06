# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
|Function|Returns|Description|
|---|---|---|
|FormatFloat(<br/>val : float,<br/>decimals : int<br/>)|[String](../static/String.md)|Formats a float to a string with the specified number of decimal places.|
|FormatFromList(<br/>str : [String](../static/String.md),<br/>list : [List](../objects/List.md)<br/>)|[String](../static/String.md)|Equivalent to C# string.format(string, List<string>).|
|Split(<br/>toSplit : [String](../static/String.md),<br/>splitter : Object,<br/>removeEmptyEntries : bool = False<br/>)|[List](../objects/List.md)|Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.|
|Join(<br/>list : [List](../objects/List.md),<br/>separator : [String](../static/String.md)<br/>)|[String](../static/String.md)|Joins a list of strings into a single string with the specified separator.|
|Substring(<br/>str : [String](../static/String.md),<br/>startIndex : int<br/>)|[String](../static/String.md)|Returns a substring starting from the specified index.|
|SubstringWithLength(<br/>str : [String](../static/String.md),<br/>startIndex : int,<br/>length : int<br/>)|[String](../static/String.md)|Returns a substring of the specified length starting from the specified start index.|
|Length(str : [String](../static/String.md))|int|Length of the string.|
|Replace(<br/>str : [String](../static/String.md),<br/>replace : [String](../static/String.md),<br/>with : [String](../static/String.md)<br/>)|[String](../static/String.md)|Replaces all occurrences of a substring with another substring.|
|Contains(<br/>str : [String](../static/String.md),<br/>match : [String](../static/String.md)<br/>)|bool|Checks if the string contains the specified substring.|
|StartsWith(<br/>str : [String](../static/String.md),<br/>match : [String](../static/String.md)<br/>)|bool|Checks if the string starts with the specified substring.|
|EndsWith(<br/>str : [String](../static/String.md),<br/>match : [String](../static/String.md)<br/>)|bool|Checks if the string ends with the specified substring.|
|Trim(str : [String](../static/String.md))|[String](../static/String.md)|Trims whitespace from the start and end of the string.|
|Insert(<br/>str : [String](../static/String.md),<br/>insert : [String](../static/String.md),<br/>index : int<br/>)|[String](../static/String.md)|Inserts a substring at the specified index.|
|Capitalize(str : [String](../static/String.md))|[String](../static/String.md)|Capitalizes the first letter of the string.|
|ToUpper(str : [String](../static/String.md))|[String](../static/String.md)|Converts the string to uppercase.|
|ToLower(str : [String](../static/String.md))|[String](../static/String.md)|Converts the string to lowercase.|
|IndexOf(<br/>str : [String](../static/String.md),<br/>substring : [String](../static/String.md)<br/>)|int|Returns the index of the given string.|
