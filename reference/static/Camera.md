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
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetManual</span>(<span style="color:blue;">bool</span> manual)
> Sets the camera manual mode. If true, camera will only be controlled by custom logic. If false, camera will follow the spawned or spectated player and read input.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetPosition</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position)
> Sets camera position.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetRotation</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> rotation)
> Sets camera rotation.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetVelocity</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> velocity)
> Sets camera velocity.
#### <span style="color:blue;">void</span> <span style="color:yellow;">LookAt</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position)
> Sets the camera forward direction such that it is looking at a world position.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetFOV</span>(<span style="color:blue;">float</span> fov)
> Sets the camera field of view. Use 0 to use the default field of view.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetCameraMode</span>(<span style="color:blue;">[String](../static/String.md)</span> mode)
> Forces the player to use a certain camera mode, taking priority over their camera setting. Accepted values are TPS, Original, FPS.
#### <span style="color:blue;">void</span> <span style="color:yellow;">ResetDistance</span>()
> Resets the follow distance to player's settings.
#### <span style="color:blue;">void</span> <span style="color:yellow;">ResetCameraMode</span>()
> Resets the camera mode to player's settings.

---

