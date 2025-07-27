# Color
Inherits from [Object](../objects/Object.md)

Represents a color.

### Remarks
Implements `__Copy__` which means that this class will act like a struct.

Overloads operators: 
- `==`
- `__Hash__`
- `__Copy__`
- `__Str__`
- `+`
- `-`
- `*`
- `/`
### Example
```csharp
Game.Print(color.ToHexString()) // Prints the color in hex format
```
### Initialization
```csharp
Color() # Default constructor, creates a white color.
Color(hexString: string) # Creates a color from a hex string
Color(r: int, g: int, b: int) # Creates a color from RGB
Color(r: int, g: int, b: int, a: int) # Creates a color from RGBA
```

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|R|int|False|Red component of the color|
|G|int|False|Green component of the color|
|B|int|False|Blue component of the color|
|A|int|False|Alpha component of the color|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function ToHexString() -> string</code></pre>
> Converts the color to a hex string


### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Lerp(a: <a data-footnote-ref href="#user-content-fn-Color">Color</a>, b: <a data-footnote-ref href="#user-content-fn-Color">Color</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-Color">Color</a></code></pre>
> Linearly interpolates between colors `a` and `b` by `t`

> **Parameters**:
> - `a`: Color to interpolate from
> - `b`: Color to interpolate to
> - `t`: Interpolation factor. 0 = `a`, 1 = `b`

> **Returns**: A new color between `a` and `b`
<pre class="language-typescript"><code class="lang-typescript">function Gradient(a: <a data-footnote-ref href="#user-content-fn-Color">Color</a>, b: <a data-footnote-ref href="#user-content-fn-Color">Color</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-Color">Color</a></code></pre>
> Creates a gradient color from two colors


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
