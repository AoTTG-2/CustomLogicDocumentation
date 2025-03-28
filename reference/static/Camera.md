# Camera
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|IsManual|bool|False|Is camera in manual mode.|
|Position|[Vector3](../objects/Vector3.md)|False|Position of the camera.|
|Rotation|[Vector3](../objects/Vector3.md)|False|Rotation of the camera.|
|Velocity|[Vector3](../objects/Vector3.md)|False|Velocity of the camera.|
|FOV|float|False|Field of view of the camera.|
|CameraMode|[String](../static/String.md)|False|Current camera mode.|
|Forward|[Vector3](../objects/Vector3.md)|False|Forward vector of the camera.|
|Right|[Vector3](../objects/Vector3.md)|False|Right vector of the camera.|
|Up|[Vector3](../objects/Vector3.md)|False|Up vector of the camera.|
|FollowDistance|float|False|Distance from the camera to the character.|
## Static Methods
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetManual</mark>(<mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">manual</mark>)
Sets the camera manual mode. If true, camera will only be controlled by custom logic. If false, camera will follow the spawned or spectated player and read input.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetPosition</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>)
Sets camera position.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetRotation</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">rotation</mark>)
Sets camera rotation.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetVelocity</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">velocity</mark>)
Sets camera velocity.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">LookAt</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>)
Sets the camera forward direction such that it is looking at a world position.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetFOV</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">fov</mark>)
Sets the camera field of view. Use 0 to use the default field of view.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetCameraMode</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">mode</mark>)
Forces the player to use a certain camera mode, taking priority over their camera setting. Accepted values are TPS, Original, FPS.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ResetDistance</mark>()
Resets the follow distance to player's settings.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ResetCameraMode</mark>()
Resets the camera mode to player's settings.

---

