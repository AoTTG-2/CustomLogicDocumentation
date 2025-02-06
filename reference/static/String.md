# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
|Function|Returns|Description|
|---|---|---|
|FormatFloat(<br/><i>val</i> : float,<br/><i>decimals</i> : int<br/>)|[String](../static/String.md)|Formats a float to a string with the specified number of decimal places.|
|FormatFromList(<br/><i>str</i> : [String](../static/String.md),<br/><i>list</i> : [List](../objects/List.md)<br/>)|[String](../static/String.md)|Equivalent to C# string.format(string, List<string>).|
|Split(<br/><i>toSplit</i> : [String](../static/String.md),<br/><i>splitter</i> : Object,<br/><i>removeEmptyEntries</i> : bool = False<br/>)|[List](../objects/List.md)|Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.|
|Join(<br/><i>list</i> : [List](../objects/List.md),<br/><i>separator</i> : [String](../static/String.md)<br/>)|[String](../static/String.md)|Joins a list of strings into a single string with the specified separator.|
|Substring(<br/><i>str</i> : [String](../static/String.md),<br/><i>startIndex</i> : int<br/>)|[String](../static/String.md)|Returns a substring starting from the specified index.|
|SubstringWithLength(<br/><i>str</i> : [String](../static/String.md),<br/><i>startIndex</i> : int,<br/><i>length</i> : int<br/>)|[String](../static/String.md)|Returns a substring of the specified length starting from the specified start index.|
|Length(<i>str</i> : [String](../static/String.md))|int|Length of the string.|
|Replace(<br/><i>str</i> : [String](../static/String.md),<br/><i>replace</i> : [String](../static/String.md),<br/><i>with</i> : [String](../static/String.md)<br/>)|[String](../static/String.md)|Replaces all occurrences of a substring with another substring.|
|Contains(<br/><i>str</i> : [String](../static/String.md),<br/><i>match</i> : [String](../static/String.md)<br/>)|bool|Checks if the string contains the specified substring.|
|StartsWith(<br/><i>str</i> : [String](../static/String.md),<br/><i>match</i> : [String](../static/String.md)<br/>)|bool|Checks if the string starts with the specified substring.|
|EndsWith(<br/><i>str</i> : [String](../static/String.md),<br/><i>match</i> : [String](../static/String.md)<br/>)|bool|Checks if the string ends with the specified substring.|
|Trim(<i>str</i> : [String](../static/String.md))|[String](../static/String.md)|Trims whitespace from the start and end of the string.|
|Insert(<br/><i>str</i> : [String](../static/String.md),<br/><i>insert</i> : [String](../static/String.md),<br/><i>index</i> : int<br/>)|[String](../static/String.md)|Inserts a substring at the specified index.|
|Capitalize(<i>str</i> : [String](../static/String.md))|[String](../static/String.md)|Capitalizes the first letter of the string.|
|ToUpper(<i>str</i> : [String](../static/String.md))|[String](../static/String.md)|Converts the string to uppercase.|
|ToLower(<i>str</i> : [String](../static/String.md))|[String](../static/String.md)|Converts the string to lowercase.|
|IndexOf(<br/><i>str</i> : [String](../static/String.md),<br/><i>substring</i> : [String](../static/String.md)<br/>)|int|Returns the index of the given string.|
