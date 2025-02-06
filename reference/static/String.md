# String
Inherits from object
## Static Fields
|<div style="width:30%">Field</div>|<div style="width:10%">Type</div>|<div style="width:10%">Readonly</div>|<div style="width:50%">Description</div>|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|FormatFloat(val : float,
decimals : int)|[String](../static/String.md)|Formats a float to a string with the specified number of decimal places.|
|FormatFromList(str : [String](../static/String.md),
list : [List](../objects/List.md))|[String](../static/String.md)|Equivalent to C# string.format(string, List<string>).|
|Split(toSplit : [String](../static/String.md),
splitter : Object,
removeEmptyEntries : bool = False)|[List](../objects/List.md)|Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.|
|Join(list : [List](../objects/List.md),
separator : [String](../static/String.md))|[String](../static/String.md)|Joins a list of strings into a single string with the specified separator.|
|Substring(str : [String](../static/String.md),
startIndex : int)|[String](../static/String.md)|Returns a substring starting from the specified index.|
|SubstringWithLength(str : [String](../static/String.md),
startIndex : int,
length : int)|[String](../static/String.md)|Returns a substring of the specified length starting from the specified start index.|
|Length(str : [String](../static/String.md))|int|Length of the string.|
|Replace(str : [String](../static/String.md),
replace : [String](../static/String.md),
with : [String](../static/String.md))|[String](../static/String.md)|Replaces all occurrences of a substring with another substring.|
|Contains(str : [String](../static/String.md),
match : [String](../static/String.md))|bool|Checks if the string contains the specified substring.|
|StartsWith(str : [String](../static/String.md),
match : [String](../static/String.md))|bool|Checks if the string starts with the specified substring.|
|EndsWith(str : [String](../static/String.md),
match : [String](../static/String.md))|bool|Checks if the string ends with the specified substring.|
|Trim(str : [String](../static/String.md))|[String](../static/String.md)|Trims whitespace from the start and end of the string.|
|Insert(str : [String](../static/String.md),
insert : [String](../static/String.md),
index : int)|[String](../static/String.md)|Inserts a substring at the specified index.|
|Capitalize(str : [String](../static/String.md))|[String](../static/String.md)|Capitalizes the first letter of the string.|
|ToUpper(str : [String](../static/String.md))|[String](../static/String.md)|Converts the string to uppercase.|
|ToLower(str : [String](../static/String.md))|[String](../static/String.md)|Converts the string to lowercase.|
|IndexOf(str : [String](../static/String.md),
substring : [String](../static/String.md))|int|Returns the index of the given string.|
