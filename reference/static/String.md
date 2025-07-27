# String
Inherits from [Object](../md/objects/Object.md)

String manipulation functions.

### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Newline|string|True|Returns the newline character.|


### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function FormatFloat(val: float, decimals: int) -> string</code></pre>
> Formats a float to a string with the specified number of decimal places.

<pre class="language-typescript"><code class="lang-typescript">function FormatFromList(str: string, list: <a data-footnote-ref href="#user-content-fn-List">List</a>) -> string</code></pre>
> Equivalent to C# string.format(string, List<string>).

<pre class="language-typescript"><code class="lang-typescript">function Split(toSplit: string, splitter: <a data-footnote-ref href="#user-content-fn-Object">Object</a>, [removeEmptyEntries: bool = False]) -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Split the string into a list. Can pass in either a string to split on or a list of strings to split on, the last optional param can remove all empty entries.

<pre class="language-typescript"><code class="lang-typescript">function Join(list: <a data-footnote-ref href="#user-content-fn-List">List</a>, separator: string) -> string</code></pre>
> Joins a list of strings into a single string with the specified separator.

<pre class="language-typescript"><code class="lang-typescript">function Substring(str: string, startIndex: int) -> string</code></pre>
> Returns a substring starting from the specified index.

<pre class="language-typescript"><code class="lang-typescript">function SubstringWithLength(str: string, startIndex: int, length: int) -> string</code></pre>
> Returns a substring of the specified length starting from the specified start index.

<pre class="language-typescript"><code class="lang-typescript">function Length(str: string) -> int</code></pre>
> Length of the string.

<pre class="language-typescript"><code class="lang-typescript">function Replace(str: string, replace: string, with: string) -> string</code></pre>
> Replaces all occurrences of a substring with another substring.

<pre class="language-typescript"><code class="lang-typescript">function Contains(str: string, match: string) -> bool</code></pre>
> Checks if the string contains the specified substring.

<pre class="language-typescript"><code class="lang-typescript">function StartsWith(str: string, match: string) -> bool</code></pre>
> Checks if the string starts with the specified substring.

<pre class="language-typescript"><code class="lang-typescript">function EndsWith(str: string, match: string) -> bool</code></pre>
> Checks if the string ends with the specified substring.

<pre class="language-typescript"><code class="lang-typescript">function Trim(str: string) -> string</code></pre>
> Trims whitespace from the start and end of the string.

<pre class="language-typescript"><code class="lang-typescript">function Insert(str: string, insert: string, index: int) -> string</code></pre>
> Inserts a substring at the specified index.

<pre class="language-typescript"><code class="lang-typescript">function Capitalize(str: string) -> string</code></pre>
> Capitalizes the first letter of the string.

<pre class="language-typescript"><code class="lang-typescript">function ToUpper(str: string) -> string</code></pre>
> Converts the string to uppercase.

<pre class="language-typescript"><code class="lang-typescript">function ToLower(str: string) -> string</code></pre>
> Converts the string to lowercase.

<pre class="language-typescript"><code class="lang-typescript">function IndexOf(str: string, substring: string) -> int</code></pre>
> Returns the index of the given string.


[^Camera]: [Camera](../md/static/Camera.md)
[^Character]: [Character](../md/objects/Character.md)
[^Collider]: [Collider](../md/objects/Collider.md)
[^Collision]: [Collision](../md/objects/Collision.md)
[^Color]: [Color](../md/objects/Color.md)
[^Convert]: [Convert](../md/static/Convert.md)
[^Cutscene]: [Cutscene](../md/static/Cutscene.md)
[^Dict]: [Dict](../md/objects/Dict.md)
[^Game]: [Game](../md/static/Game.md)
[^Human]: [Human](../md/objects/Human.md)
[^Input]: [Input](../md/static/Input.md)
[^Json]: [Json](../md/static/Json.md)
[^LineCastHitResult]: [LineCastHitResult](../md/objects/LineCastHitResult.md)
[^LineRenderer]: [LineRenderer](../md/objects/LineRenderer.md)
[^List]: [List](../md/objects/List.md)
[^Map]: [Map](../md/static/Map.md)
[^MapObject]: [MapObject](../md/objects/MapObject.md)
[^MapTargetable]: [MapTargetable](../md/objects/MapTargetable.md)
[^Math]: [Math](../md/static/Math.md)
[^Network]: [Network](../md/static/Network.md)
[^NetworkView]: [NetworkView](../md/objects/NetworkView.md)
[^PersistentData]: [PersistentData](../md/static/PersistentData.md)
[^Physics]: [Physics](../md/static/Physics.md)
[^Player]: [Player](../md/objects/Player.md)
[^Quaternion]: [Quaternion](../md/objects/Quaternion.md)
[^Random]: [Random](../md/objects/Random.md)
[^Range]: [Range](../md/objects/Range.md)
[^RoomData]: [RoomData](../md/static/RoomData.md)
[^Set]: [Set](../md/objects/Set.md)
[^Shifter]: [Shifter](../md/objects/Shifter.md)
[^String]: [String](../md/static/String.md)
[^Time]: [Time](../md/static/Time.md)
[^Titan]: [Titan](../md/objects/Titan.md)
[^Transform]: [Transform](../md/objects/Transform.md)
[^UI]: [UI](../md/static/UI.md)
[^Vector2]: [Vector2](../md/objects/Vector2.md)
[^Vector3]: [Vector3](../md/objects/Vector3.md)
[^Object]: [Object](../md/objects/Object.md)
[^Component]: [Component](../md/objects/Component.md)
