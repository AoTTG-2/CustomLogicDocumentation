# Camera
Inherits from object
## Static Fields
|<div style="width:30%">Field</div>|<div style="width:10%">Type</div>|<div style="width:10%">Readonly</div>|<div style="width:50%">Description</div>|
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
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|SetManual(manual : bool)|none|Sets the camera manual mode. If true, camera will only be controlled by custom logic. If false, camera will follow the spawned or spectated player and read input.|
|SetPosition(position : [Vector3](../objects/Vector3.md))|none|Sets camera position.|
|SetRotation(rotation : [Vector3](../objects/Vector3.md))|none|Sets camera rotation.|
|SetVelocity(velocity : [Vector3](../objects/Vector3.md))|none|Sets camera velocity.|
|LookAt(position : [Vector3](../objects/Vector3.md))|none|Sets the camera forward direction such that it is looking at a world position.|
|SetFOV(fov : float)|none|Sets the camera field of view. Use 0 to use the default field of view.|
|SetCameraMode(mode : [String](../static/String.md))|none|Forces the player to use a certain camera mode, taking priority over their camera setting. Accepted values are TPS, Original, FPS.|
|ResetDistance()|none|Resets the follow distance to player's settings.|
|ResetCameraMode()|none|Resets the camera mode to player's settings.|
