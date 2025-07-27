# Vector2
Inherits from [Object](../md/objects/Object.md)
### Remarks
Overloads operators: 
- `__Copy__`
- `+`
- `-`
- `*`
- `/`
- `==`
- `__Hash__`
### Initialization
```csharp
Vector2()
Vector2(xy: float)
Vector2(x: float, y: float)
```

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|X|float|False|X component of the vector.|
|Y|float|False|Y component of the vector.|
|Normalized|[Vector2](../md/objects/Vector2.md)|True|Returns this vector with a magnitude of 1 (Read Only).|
|Magnitude|float|True|Returns the length of this vector (Read Only).|
|SqrMagnitude|float|True|Returns the squared length of this vector (Read Only).|


### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Zero|[Vector2](../md/objects/Vector2.md)|True|Shorthand for writing Vector2(0, 0).|
|One|[Vector2](../md/objects/Vector2.md)|True|Shorthand for writing Vector2(1, 1).|
|Up|[Vector2](../md/objects/Vector2.md)|True|Shorthand for writing Vector2(0, 1).|
|Down|[Vector2](../md/objects/Vector2.md)|True|Shorthand for writing Vector2(0, -1).|
|Left|[Vector2](../md/objects/Vector2.md)|True|Shorthand for writing Vector2(-1, 0).|
|Right|[Vector2](../md/objects/Vector2.md)|True|Shorthand for writing Vector2(1, 0).|
|NegativeInfinity|[Vector2](../md/objects/Vector2.md)|True|Shorthand for writing Vector2(float.PositiveInfinity, float.PositiveInfinity).|
|PositiveInfinity|[Vector2](../md/objects/Vector2.md)|True|Shorthand for writing Vector2(float.PositiveInfinity, float.PositiveInfinity).|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Set(x: float, y: float) -> null</code></pre>
> Set x and y components of an existing Vector2.

<pre class="language-typescript"><code class="lang-typescript">function Normalize() -> null</code></pre>
> Makes this vector have a magnitude of 1.


### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Angle(from: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, to: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>) -> float</code></pre>
> Gets the unsigned angle in degrees between from and to.

> **Returns**: The unsigned angle in degrees between the two vectors.
<pre class="language-typescript"><code class="lang-typescript">function ClampMagnitude(vector: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, maxLength: float) -> <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a></code></pre>
> Returns a copy of vector with its magnitude clamped to maxLength.

<pre class="language-typescript"><code class="lang-typescript">function Distance(a: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, b: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>) -> float</code></pre>
> Returns the distance between a and b.

<pre class="language-typescript"><code class="lang-typescript">function Dot(a: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, b: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>) -> float</code></pre>
> Dot Product of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Lerp(a: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, b: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a></code></pre>
> Linearly interpolates between vectors a and b by t.

<pre class="language-typescript"><code class="lang-typescript">function LerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, b: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a></code></pre>
> Linearly interpolates between vectors a and b by t.

<pre class="language-typescript"><code class="lang-typescript">function Max(a: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, b: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>) -> <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a></code></pre>
> Returns a vector that is made from the largest components of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Min(a: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, b: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>) -> <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a></code></pre>
> Returns a vector that is made from the smallest components of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function MoveTowards(current: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, target: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, maxDistanceDelta: float) -> <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a></code></pre>
> Moves a point current towards target.

<pre class="language-typescript"><code class="lang-typescript">function Reflect(inDirection: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, inNormal: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>) -> <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a></code></pre>
> Reflects a vector off the vector defined by a normal.

<pre class="language-typescript"><code class="lang-typescript">function SignedAngle(from: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, to: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>) -> float</code></pre>
> Gets the signed angle in degrees between from and to.

> **Returns**: The signed angle in degrees between the two vectors.
<pre class="language-typescript"><code class="lang-typescript">function SmoothDamp(current: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, target: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, currentVelocity: <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a>, smoothTime: float, maxSpeed: float) -> <a data-footnote-ref href="#user-content-fn-Vector2">Vector2</a></code></pre>

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
