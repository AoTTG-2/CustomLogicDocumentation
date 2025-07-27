# PersistentData
Inherits from [Object](../md/objects/Object.md)

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
