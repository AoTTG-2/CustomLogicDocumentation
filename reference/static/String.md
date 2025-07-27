# String
Inherits from [Object](../objects/Object.md)

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


[^Camera]: [Camera](../static/Camera.md)
[^Character]: [Character](../objects/Character.md)
[^Collider]: [Collider](../objects/Collider.md)
[^Collision]: [Collision](../objects/Collision.md)
[^Color]: [Color](../objects/Color.md)
[^Convert]: [Convert](../static/Convert.md)
[^Cutscene]: [Cutscene](../static/Cutscene.md)
[^Dict]: [Dict](../objects/Dict.md)
[^Game]: [Game](../static/Game.md)
[^Human]: [Human](../objects/Human.md)
[^Input]: [Input](../static/Input.md)
[^Json]: [Json](../static/Json.md)
[^LineCastHitResult]: [LineCastHitResult](../objects/LineCastHitResult.md)
[^LineRenderer]: [LineRenderer](../objects/LineRenderer.md)
[^List]: [List](../objects/List.md)
[^Map]: [Map](../static/Map.md)
[^MapObject]: [MapObject](../objects/MapObject.md)
[^MapTargetable]: [MapTargetable](../objects/MapTargetable.md)
[^Math]: [Math](../static/Math.md)
[^Network]: [Network](../static/Network.md)
[^NetworkView]: [NetworkView](../objects/NetworkView.md)
[^PersistentData]: [PersistentData](../static/PersistentData.md)
[^Physics]: [Physics](../static/Physics.md)
[^Player]: [Player](../objects/Player.md)
[^Quaternion]: [Quaternion](../objects/Quaternion.md)
[^Random]: [Random](../objects/Random.md)
[^Range]: [Range](../objects/Range.md)
[^RoomData]: [RoomData](../static/RoomData.md)
[^Set]: [Set](../objects/Set.md)
[^Shifter]: [Shifter](../objects/Shifter.md)
[^String]: [String](../static/String.md)
[^Time]: [Time](../static/Time.md)
[^Titan]: [Titan](../objects/Titan.md)
[^Transform]: [Transform](../objects/Transform.md)
[^UI]: [UI](../static/UI.md)
[^Vector2]: [Vector2](../objects/Vector2.md)
[^Vector3]: [Vector3](../objects/Vector3.md)
[^Object]: [Object](../objects/Object.md)
[^Component]: [Component](../objects/Component.md)
