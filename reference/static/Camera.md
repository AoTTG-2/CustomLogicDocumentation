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
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetManual</mark>(<mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">manual</mark>)
Sets the camera manual mode. If true, camera will only be controlled by custom logic. If false, camera will follow the spawned or spectated player and read input.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetPosition</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">position</mark>)
Sets camera position.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetRotation</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">rotation</mark>)
Sets camera rotation.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetVelocity</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">velocity</mark>)
Sets camera velocity.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">LookAt</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">position</mark>)
Sets the camera forward direction such that it is looking at a world position.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetFOV</mark>(<mark style="color:Blue;">float</mark> <mark style="color:Yellow;">fov</mark>)
Sets the camera field of view. Use 0 to use the default field of view.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetCameraMode</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">mode</mark>)
Forces the player to use a certain camera mode, taking priority over their camera setting. Accepted values are TPS, Original, FPS.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">ResetDistance</mark>()
Resets the follow distance to player's settings.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">ResetCameraMode</mark>()
Resets the camera mode to player's settings.

---

