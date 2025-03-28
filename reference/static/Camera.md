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
#### void <span style="color":#dcdcaa>SetManual<span>(bool <span style="color":#9cdcfe>manual<span>)
Sets the camera manual mode. If true, camera will only be controlled by custom logic. If false, camera will follow the spawned or spectated player and read input.
#### void <span style="color":#dcdcaa>SetPosition<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>)
Sets camera position.
#### void <span style="color":#dcdcaa>SetRotation<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>rotation<span>)
Sets camera rotation.
#### void <span style="color":#dcdcaa>SetVelocity<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>velocity<span>)
Sets camera velocity.
#### void <span style="color":#dcdcaa>LookAt<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>)
Sets the camera forward direction such that it is looking at a world position.
#### void <span style="color":#dcdcaa>SetFOV<span>(float <span style="color":#9cdcfe>fov<span>)
Sets the camera field of view. Use 0 to use the default field of view.
#### void <span style="color":#dcdcaa>SetCameraMode<span>([String](../static/String.md) <span style="color":#9cdcfe>mode<span>)
Forces the player to use a certain camera mode, taking priority over their camera setting. Accepted values are TPS, Original, FPS.
#### void <span style="color":#dcdcaa>ResetDistance<span>()
Resets the follow distance to player's settings.
#### void <span style="color":#dcdcaa>ResetCameraMode<span>()
Resets the camera mode to player's settings.

---

