# Random
Inherits from [Object](../objects/Object.md)

Random can be initialized as a class with an int given as the seed value.
Note that this is optional, and you can reference Random directly as a static class.

### Example
```csharp
# Use random methods directly
r = Random.RandomInt(0, 100);

# Or create an instance of Random with a seed
generator = Random(123);

# Use it
a = generator.RandomInt(0, 100);

# Seed allows repeatable random values
generator2 = Random(123);
b = generator.RandomInt(0, 100);
compared = a == b;    # Always True
```
### Initialization
```csharp
Random()
Random(seed: int)
```

### Methods
<pre class="language-typescript"><code class="lang-typescript">function RandomInt(min: int, max: int) -> int</code></pre>
> Generates a random integer between the specified range.

<pre class="language-typescript"><code class="lang-typescript">function RandomFloat(min: float, max: float) -> float</code></pre>
> Generates a random float between the specified range.

<pre class="language-typescript"><code class="lang-typescript">function RandomBool() -> bool</code></pre>
> Returns random boolean.

<pre class="language-typescript"><code class="lang-typescript">function RandomVector3(a: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Generates a random Vector3 between the specified ranges.

<pre class="language-typescript"><code class="lang-typescript">function RandomDirection([flat: bool = False]) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Generates a random normalized direction vector. If flat is true, the y component will be zero.

<pre class="language-typescript"><code class="lang-typescript">function RandomSign() -> int</code></pre>
> Generates a random sign, either 1 or -1.

<pre class="language-typescript"><code class="lang-typescript">function PerlinNoise(x: float, y: float) -> float</code></pre>
> Returns a point sampled from generated 2d perlin noise. (see Unity Mathf.PerlinNoise for more information)


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
