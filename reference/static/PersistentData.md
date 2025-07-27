# PersistentData
Inherits from [Object](../objects/Object.md)

Store and retrieve persistent data. Persistent data can be saved and loaded from file. Supports float, int, string, and bool types.
Note that any game mode may use the same file names, so it is recommended that you choose unique file names when saving and loading.
Saved files are located in Documents/Aottg2/PersistentData.

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function SetProperty(property: string, value: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Sets the property with given name to the object value. Valid value types are float, string, bool, and int.

<pre class="language-typescript"><code class="lang-typescript">function GetProperty(property: string, defaultValue: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> <a data-footnote-ref href="#user-content-fn-Object">Object</a></code></pre>
> Gets the property with given name. If property does not exist, returns defaultValue.

<pre class="language-typescript"><code class="lang-typescript">function LoadFromFile(fileName: string, encrypted: bool) -> null</code></pre>
> Loads persistent data from given file name. If encrypted is true, will treat the file as having been saved as encrypted.

<pre class="language-typescript"><code class="lang-typescript">function SaveToFile(fileName: string, encrypted: bool) -> null</code></pre>
> Saves current persistent data to given file name. If encrypted is true, will also encrypt the file instead of using plaintext.

<pre class="language-typescript"><code class="lang-typescript">function Clear() -> null</code></pre>
> Clears current persistent data.

<pre class="language-typescript"><code class="lang-typescript">function IsValidFileName(fileName: string) -> bool</code></pre>
> Determines whether or not the given fileName will be allowed for use when saving/loading a file.

<pre class="language-typescript"><code class="lang-typescript">function FileExists(fileName: string) -> bool</code></pre>
> Determines whether the file given already exists. Throws an error if given an invalid file name.


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
