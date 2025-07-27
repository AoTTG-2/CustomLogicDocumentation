# Input
Inherits from [Object](../md/objects/Object.md)

Reading player key inputs. Note that inputs are best handled in OnFrame rather than OnTick, due to being updated every frame and not every physics tick.

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function GetKeyName(key: string) -> string</code></pre>
> Gets the key name the player assigned to the key setting

<pre class="language-typescript"><code class="lang-typescript">function GetKeyHold(key: string) -> bool</code></pre>
> Returns true if the key is being held down

<pre class="language-typescript"><code class="lang-typescript">function GetKeyDown(key: string) -> bool</code></pre>
> Returns true if the key was pressed down this frame

<pre class="language-typescript"><code class="lang-typescript">function GetKeyUp(key: string) -> bool</code></pre>
> Returns true if the key was released this frame

<pre class="language-typescript"><code class="lang-typescript">function GetMouseAim() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Returns the position the player is aiming at

<pre class="language-typescript"><code class="lang-typescript">function GetCursorAimDirection() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Returns the ray the player is aiming at

<pre class="language-typescript"><code class="lang-typescript">function GetMouseSpeed() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Returns the speed of the mouse

<pre class="language-typescript"><code class="lang-typescript">function GetMousePosition() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Returns the position of the mouse

<pre class="language-typescript"><code class="lang-typescript">function GetScreenDimensions() -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Returns the dimensions of the screen

<pre class="language-typescript"><code class="lang-typescript">function SetKeyDefaultEnabled(key: string, enabled: bool) -> null</code></pre>
> Sets whether the key is enabled by default

<pre class="language-typescript"><code class="lang-typescript">function SetKeyHold(key: string, enabled: bool) -> null</code></pre>
> Sets whether the key is being held down


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
