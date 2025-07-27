# Transform
Inherits from [Object](../md/objects/Object.md)
### Remarks
Overloads operators: 
- `==`
- `__Hash__`
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Position|[Vector3](../md/objects/Vector3.md)|False|Gets or sets the position of the transform.|
|LocalPosition|[Vector3](../md/objects/Vector3.md)|False|Gets or sets the local position of the transform.|
|Rotation|[Vector3](../md/objects/Vector3.md)|False|Gets or sets the rotation of the transform.|
|LocalRotation|[Vector3](../md/objects/Vector3.md)|False|Gets or sets the local rotation of the transform.|
|QuaternionRotation|[Quaternion](../md/objects/Quaternion.md)|False|Gets or sets the quaternion rotation of the transform.|
|QuaternionLocalRotation|[Quaternion](../md/objects/Quaternion.md)|False|Gets or sets the quaternion local rotation of the transform.|
|Scale|[Vector3](../md/objects/Vector3.md)|False|Gets or sets the scale of the transform.|
|Forward|[Vector3](../md/objects/Vector3.md)|False|Gets the forward vector of the transform.|
|Up|[Vector3](../md/objects/Vector3.md)|False|Gets the up vector of the transform.|
|Right|[Vector3](../md/objects/Vector3.md)|False|Gets the right vector of the transform.|
|Name|string|True|Gets the name of the transform.|
|Layer|int|False|Gets the Physics Layer of the transform.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function GetTransform(name: string) -> <a data-footnote-ref href="#user-content-fn-Transform">Transform</a></code></pre>
> Gets the transform of the specified child.

<pre class="language-typescript"><code class="lang-typescript">function GetTransforms() -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Gets all child transforms.

<pre class="language-typescript"><code class="lang-typescript">function PlayAnimation(anim: string, [fade: float = 0.1]) -> null</code></pre>
> Plays the specified animation.

<pre class="language-typescript"><code class="lang-typescript">function PlayAnimationAt(anim: string, normalizedTime: float, [fade: float = 0.1]) -> null</code></pre>
> Plays the specified animation starting from a normalized time.

<pre class="language-typescript"><code class="lang-typescript">function SetAnimationSpeed(speed: float) -> null</code></pre>
> Sets the animation playback speed

<pre class="language-typescript"><code class="lang-typescript">function GetAnimationLength(anim: string) -> float</code></pre>
> Gets the length of the specified animation.

<pre class="language-typescript"><code class="lang-typescript">function PlaySound() -> null</code></pre>
> Plays the sound.

<pre class="language-typescript"><code class="lang-typescript">function StopSound() -> null</code></pre>
> Stops the sound.

<pre class="language-typescript"><code class="lang-typescript">function ToggleParticle(enabled: bool) -> null</code></pre>
> Toggles the particle system.

<pre class="language-typescript"><code class="lang-typescript">function InverseTransformDirection(direction: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Transforms a direction from world space to local space. The opposite of Transform.TransformDirection.

<pre class="language-typescript"><code class="lang-typescript">function InverseTransformPoint(point: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Transforms position from world space to local space.

<pre class="language-typescript"><code class="lang-typescript">function TransformDirection(direction: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Transforms direction from local space to world space.

<pre class="language-typescript"><code class="lang-typescript">function TransformPoint(point: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a></code></pre>
> Transforms position from local space to world space.

<pre class="language-typescript"><code class="lang-typescript">function Rotate(rotation: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> null</code></pre>
> Applies a rotation of eulerAngles.z degrees around the z-axis, eulerAngles.x degrees around the x-axis, and eulerAngles.y degrees around the y-axis (in that order).

<pre class="language-typescript"><code class="lang-typescript">function RotateAround(point: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, axis: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, angle: float) -> null</code></pre>
> Rotates the transform about axis passing through point in world coordinates by angle degrees.

<pre class="language-typescript"><code class="lang-typescript">function LookAt(target: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> null</code></pre>
> Rotates the transform so the forward vector points at worldPosition.

<pre class="language-typescript"><code class="lang-typescript">function SetRenderersEnabled(enabled: bool) -> null</code></pre>
> Sets the enabled state of all child renderers.

<pre class="language-typescript"><code class="lang-typescript">function GetColliders([recursive: bool = False]) -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Gets colliders of the transform.


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
