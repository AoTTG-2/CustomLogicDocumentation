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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetManual</mark>(<mark style="color:blue;">bool</mark> manual)
> Sets the camera manual mode. If true, camera will only be controlled by custom logic. If false, camera will follow the spawned or spectated player and read input.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetPosition</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> position)
> Sets camera position.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetRotation</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> rotation)
> Sets camera rotation.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetVelocity</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> velocity)
> Sets camera velocity.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">LookAt</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> position)
> Sets the camera forward direction such that it is looking at a world position.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetFOV</mark>(<mark style="color:blue;">float</mark> fov)
> Sets the camera field of view. Use 0 to use the default field of view.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetCameraMode</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> mode)
> Forces the player to use a certain camera mode, taking priority over their camera setting. Accepted values are TPS, Original, FPS.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ResetDistance</mark>()
> Resets the follow distance to player's settings.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ResetCameraMode</mark>()
> Resets the camera mode to player's settings.

---

