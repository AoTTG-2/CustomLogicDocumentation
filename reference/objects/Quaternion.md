# Quaternion
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
### Example
```csharp
# Quaternion takes four floats X, Y, Z and W as parameters when initializing.
quaternion = Quaternion(0.5, 0.5, 0.5, 0.5);
```
### Initialization
```csharp
Quaternion(parameterValues: Object)
```

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|X|float|False|X component of the Quaternion. Don't modify this directly unless you know quaternions inside out.|
|Y|float|False|Y component of the Quaternion. Don't modify this directly unless you know quaternions inside out.|
|Z|float|False|Z component of the Quaternion. Don't modify this directly unless you know quaternions inside out.|
|W|float|False|W component of the Quaternion. Do not directly modify quaternions.|
|Euler|[Vector3](../md/objects/Vector3.md)|False|Returns or sets the euler angle representation of the rotation.|


### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Identity|[Quaternion](../md/objects/Quaternion.md)|True|The identity rotation (Read Only).|


### Methods

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Lerp(a: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, b: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a></code></pre>
> Interpolates between a and b by t and normalizes the result afterwards.

> **Returns**: A unit quaternion interpolated between quaternions a and b.
<pre class="language-typescript"><code class="lang-typescript">function LerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, b: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a></code></pre>
> Interpolates between a and b by t and normalizes the result afterwards. The parameter t is not clamped.

<pre class="language-typescript"><code class="lang-typescript">function Slerp(a: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, b: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a></code></pre>
> Spherically linear interpolates between unit quaternions a and b by a ratio of t.

> **Returns**: A unit quaternion spherically interpolated between quaternions a and b.
<pre class="language-typescript"><code class="lang-typescript">function SlerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, b: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a></code></pre>
> Spherically linear interpolates between unit quaternions a and b by t.

> **Returns**: A unit quaternion spherically interpolated between unit quaternions a and b.
<pre class="language-typescript"><code class="lang-typescript">function FromEuler(euler: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a></code></pre>
> Returns the Quaternion rotation from the given euler angles.

<pre class="language-typescript"><code class="lang-typescript">function LookRotation(forward: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [upwards: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a> = null]) -> <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a></code></pre>
> Creates a rotation with the specified forward and upwards directions.

<pre class="language-typescript"><code class="lang-typescript">function FromToRotation(a: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a></code></pre>
> Creates a rotation from fromDirection to toDirection.

> **Returns**: A unit quaternion which rotates from fromDirection to toDirection.
<pre class="language-typescript"><code class="lang-typescript">function Inverse(q: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>) -> <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a></code></pre>
> Returns the Inverse of rotation.

<pre class="language-typescript"><code class="lang-typescript">function RotateTowards(from: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, to: <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a>, maxDegreesDelta: float) -> <a data-footnote-ref href="#user-content-fn-Quaternion">Quaternion</a></code></pre>
> Rotates a rotation from towards to.

> **Returns**: A unit quaternion rotated towards to by an angular step of maxDegreesDelta.

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
