# UI
Inherits from [Object](../md/objects/Object.md)

UI label functions.

### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|TopCenter|string|True|"TopCenter" constant|
|TopLeft|string|True|"TopLeft" constant|
|TopRight|string|True|"TopRight" constant|
|MiddleCenter|string|True|"MiddleCenter" constant|
|MiddleLeft|string|True|"MiddleLeft" constant|
|MiddleRight|string|True|"MiddleRight" constant|
|BottomCenter|string|True|"BottomCenter" constant|
|BottomLeft|string|True|"BottomLeft" constant|
|BottomRight|string|True|"BottomRight" constant|
|GetPopups|[List](../md/objects/List.md)|True|Returns a list of all popups|


### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function SetLabel(label: string, message: string) -> null</code></pre>
> Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".

<pre class="language-typescript"><code class="lang-typescript">function SetLabelForTime(label: string, message: string, time: float) -> null</code></pre>
> Sets the label for a certain time, after which it will be cleared.

<pre class="language-typescript"><code class="lang-typescript">function SetLabelAll(label: string, message: string) -> null</code></pre>
> Sets the label for all players. Master client only. Be careful not to call this often.

<pre class="language-typescript"><code class="lang-typescript">function SetLabelForTimeAll(label: string, message: string, time: float) -> null</code></pre>
> Sets the label for all players for a certain time. Master client only.

<pre class="language-typescript"><code class="lang-typescript">function CreatePopup(popupName: string, title: string, width: int, height: int) -> string</code></pre>
> Creates a new popup. This popup is hidden until shown.

<pre class="language-typescript"><code class="lang-typescript">function ShowPopup(popupName: string) -> null</code></pre>
> Shows the popup with given name.

<pre class="language-typescript"><code class="lang-typescript">function HidePopup(popupName: string) -> null</code></pre>
> Hides the popup with given name.

<pre class="language-typescript"><code class="lang-typescript">function ClearPopup(popupName: string) -> null</code></pre>
> Clears all elements in popup with given name.

<pre class="language-typescript"><code class="lang-typescript">function AddPopupLabel(popupName: string, label: string) -> null</code></pre>
> Adds a text row to the popup with label as content.

<pre class="language-typescript"><code class="lang-typescript">function AddPopupButton(popupName: string, label: string, callback: string) -> null</code></pre>
> Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.

<pre class="language-typescript"><code class="lang-typescript">function AddPopupBottomButton(popupName: string, label: string, callback: string) -> null</code></pre>
> Adds a button to the bottom bar of the popup.

<pre class="language-typescript"><code class="lang-typescript">function AddPopupButtons(popupName: string, labels: <a data-footnote-ref href="#user-content-fn-List">List</a>, callbacks: <a data-footnote-ref href="#user-content-fn-List">List</a>) -> null</code></pre>
> Adds a list of buttons in a row to the popup.

<pre class="language-typescript"><code class="lang-typescript">function WrapStyleTag(text: string, style: string, [arg: string = null]) -> string</code></pre>
> Returns a wrapped string given style and args.

<pre class="language-typescript"><code class="lang-typescript">function GetLocale(cat: string, sub: string, key: string) -> string</code></pre>
> Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.

<pre class="language-typescript"><code class="lang-typescript">function GetLanguage() -> string</code></pre>
> Returns the current language (e.g. "English" or "简体中文").

<pre class="language-typescript"><code class="lang-typescript">function ShowChangeCharacterMenu() -> null</code></pre>
> Shows the change character menu if main character is Human.

<pre class="language-typescript"><code class="lang-typescript">function SetScoreboardHeader(header: string) -> null</code></pre>
> Sets the display of the scoreboard header (default "Kills / Deaths...")

<pre class="language-typescript"><code class="lang-typescript">function SetScoreboardProperty(property: string) -> null</code></pre>
> Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.

<pre class="language-typescript"><code class="lang-typescript">function GetThemeColor(panel: string, category: string, item: string) -> <a data-footnote-ref href="#user-content-fn-Color">Color</a></code></pre>
> Gets the color of the specified item. See theme json for reference.

<pre class="language-typescript"><code class="lang-typescript">function IsPopupActive(popupName: string) -> bool</code></pre>
> Returns if the given popup is active


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
