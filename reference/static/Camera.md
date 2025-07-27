# Camera
Inherits from [Object](../md/objects/Object.md)

References the main game camera.

### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|IsManual|bool|True|Is camera in manual mode.|
|Position|[Vector3](../md/objects/Vector3.md)|True|Position of the camera.|
|Rotation|[Vector3](../md/objects/Vector3.md)|True|Rotation of the camera.|
|Velocity|[Vector3](../md/objects/Vector3.md)|True|Velocity of the camera.|
|FOV|float|True|Field of view of the camera.|
|CameraMode|string|True|Current camera mode.|
|Forward|[Vector3](../md/objects/Vector3.md)|False|Forward vector of the camera.|
|Right|[Vector3](../md/objects/Vector3.md)|False|Right vector of the camera.|
|Up|[Vector3](../md/objects/Vector3.md)|False|Up vector of the camera.|
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
