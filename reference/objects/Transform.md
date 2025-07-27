# Transform
Inherits from [Object](../objects/Object.md)
### Remarks
Overloads operators: 
- `==`
- `__Hash__`
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Position|[Vector3](../objects/Vector3.md)|False|Gets or sets the position of the transform.|
|LocalPosition|[Vector3](../objects/Vector3.md)|False|Gets or sets the local position of the transform.|
|Rotation|[Vector3](../objects/Vector3.md)|False|Gets or sets the rotation of the transform.|
|LocalRotation|[Vector3](../objects/Vector3.md)|False|Gets or sets the local rotation of the transform.|
|QuaternionRotation|[Quaternion](../objects/Quaternion.md)|False|Gets or sets the quaternion rotation of the transform.|
|QuaternionLocalRotation|[Quaternion](../objects/Quaternion.md)|False|Gets or sets the quaternion local rotation of the transform.|
|Scale|[Vector3](../objects/Vector3.md)|False|Gets or sets the scale of the transform.|
|Forward|[Vector3](../objects/Vector3.md)|False|Gets the forward vector of the transform.|
|Up|[Vector3](../objects/Vector3.md)|False|Gets the up vector of the transform.|
|Right|[Vector3](../objects/Vector3.md)|False|Gets the right vector of the transform.|
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
