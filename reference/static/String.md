# String
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Newline|[String](../static/String.md)|False|Returns the newline character.|
## Static Methods
#### [String](../static/String.md) <span style="color":#dcdcaa>FormatFloat<span>(float <span style="color":#9cdcfe>val<span>, int <span style="color":#9cdcfe>decimals<span>)
Formats a float to a string with the specified number of decimal places.
#### [String](../static/String.md) <span style="color":#dcdcaa>FormatFromList<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>, [List](../objects/List.md) <span style="color":#9cdcfe>list<span>)
Equivalent to C# string.format(string, List<string>).
#### [List](../objects/List.md) <span style="color":#dcdcaa>Split<span>([String](../static/String.md) <span style="color":#9cdcfe>toSplit<span>, Object <span style="color":#9cdcfe>splitter<span>, bool <span style="color":#9cdcfe>removeEmptyEntries<span> = False)
Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.
#### [String](../static/String.md) <span style="color":#dcdcaa>Join<span>([List](../objects/List.md) <span style="color":#9cdcfe>list<span>, [String](../static/String.md) <span style="color":#9cdcfe>separator<span>)
Joins a list of strings into a single string with the specified separator.
#### [String](../static/String.md) <span style="color":#dcdcaa>Substring<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>, int <span style="color":#9cdcfe>startIndex<span>)
Returns a substring starting from the specified index.
#### [String](../static/String.md) <span style="color":#dcdcaa>SubstringWithLength<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>, int <span style="color":#9cdcfe>startIndex<span>, int <span style="color":#9cdcfe>length<span>)
Returns a substring of the specified length starting from the specified start index.
#### int <span style="color":#dcdcaa>Length<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>)
Length of the string.
#### [String](../static/String.md) <span style="color":#dcdcaa>Replace<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>, [String](../static/String.md) <span style="color":#9cdcfe>replace<span>, [String](../static/String.md) <span style="color":#9cdcfe>with<span>)
Replaces all occurrences of a substring with another substring.
#### bool <span style="color":#dcdcaa>Contains<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>, [String](../static/String.md) <span style="color":#9cdcfe>match<span>)
Checks if the string contains the specified substring.
#### bool <span style="color":#dcdcaa>StartsWith<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>, [String](../static/String.md) <span style="color":#9cdcfe>match<span>)
Checks if the string starts with the specified substring.
#### bool <span style="color":#dcdcaa>EndsWith<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>, [String](../static/String.md) <span style="color":#9cdcfe>match<span>)
Checks if the string ends with the specified substring.
#### [String](../static/String.md) <span style="color":#dcdcaa>Trim<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>)
Trims whitespace from the start and end of the string.
#### [String](../static/String.md) <span style="color":#dcdcaa>Insert<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>, [String](../static/String.md) <span style="color":#9cdcfe>insert<span>, int <span style="color":#9cdcfe>index<span>)
Inserts a substring at the specified index.
#### [String](../static/String.md) <span style="color":#dcdcaa>Capitalize<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>)
Capitalizes the first letter of the string.
#### [String](../static/String.md) <span style="color":#dcdcaa>ToUpper<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>)
Converts the string to uppercase.
#### [String](../static/String.md) <span style="color":#dcdcaa>ToLower<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>)
Converts the string to lowercase.
#### int <span style="color":#dcdcaa>IndexOf<span>([String](../static/String.md) <span style="color":#9cdcfe>str<span>, [String](../static/String.md) <span style="color":#9cdcfe>substring<span>)
Returns the index of the given string.

---

