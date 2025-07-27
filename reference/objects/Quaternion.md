# Quaternion
Inherits from [Object](../objects/Object.md)
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
|Euler|[Vector3](../objects/Vector3.md)|False|Returns or sets the euler angle representation of the rotation.|


### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Identity|[Quaternion](../objects/Quaternion.md)|True|The identity rotation (Read Only).|


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
