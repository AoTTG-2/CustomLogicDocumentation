# Color
Inherits from [Object](../md/objects/Object.md)

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
