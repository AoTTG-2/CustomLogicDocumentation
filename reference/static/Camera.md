# Camera
Inherits from [Object](../objects/Object.md)

References the main game camera.

### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|IsManual|bool|True|Is camera in manual mode.|
|Position|[Vector3](../objects/Vector3.md)|True|Position of the camera.|
|Rotation|[Vector3](../objects/Vector3.md)|True|Rotation of the camera.|
|Velocity|[Vector3](../objects/Vector3.md)|True|Velocity of the camera.|
|FOV|float|True|Field of view of the camera.|
|CameraMode|string|True|Current camera mode.|
|Forward|[Vector3](../objects/Vector3.md)|False|Forward vector of the camera.|
|Right|[Vector3](../objects/Vector3.md)|False|Right vector of the camera.|
|Up|[Vector3](../objects/Vector3.md)|False|Up vector of the camera.|
|FollowDistance|float|False|Distance from the camera to the character.|


### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function SetManual(manual: bool) -> null</code></pre>
> Sets the camera manual mode. If true, camera will only be controlled by custom logic. If false, camera will follow the spawned or spectated player and read input.

<pre class="language-typescript"><code class="lang-typescript">function SetPosition(position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> null</code></pre>
> Sets camera position.

<pre class="language-typescript"><code class="lang-typescript">function SetRotation(rotation: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> null</code></pre>
> Sets camera rotation.

<pre class="language-typescript"><code class="lang-typescript">function SetVelocity(velocity: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> null</code></pre>
> Sets camera velocity.

<pre class="language-typescript"><code class="lang-typescript">function LookAt(position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> null</code></pre>
> Sets the camera forward direction such that it is looking at a world position.

<pre class="language-typescript"><code class="lang-typescript">function SetFOV(fov: float) -> null</code></pre>
> Sets the camera field of view. Use 0 to use the default field of view.

<pre class="language-typescript"><code class="lang-typescript">function SetCameraMode(mode: string) -> null</code></pre>
> Forces the player to use a certain camera mode, taking priority over their camera setting. Accepted values are TPS, Original, FPS.

<pre class="language-typescript"><code class="lang-typescript">function ResetDistance() -> null</code></pre>
> Resets the follow distance to player's settings.

<pre class="language-typescript"><code class="lang-typescript">function ResetCameraMode() -> null</code></pre>
> Resets the camera mode to player's settings.


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
