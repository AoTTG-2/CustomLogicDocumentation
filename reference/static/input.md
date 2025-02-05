# Input
Inherits from object
## Methods
|Function|Returns|Description|
|---|---|---|
|GetKeyName(key : [String](../static/string.md))|[String](../static/string.md)|Gets the key name the player assigned to the key setting|
|GetKeyHold(key : [String](../static/string.md))|bool|Returns true if the key is being held down|
|GetKeyDown(key : [String](../static/string.md))|bool|Returns true if the key was pressed down this frame|
|GetKeyUp(key : [String](../static/string.md))|bool|Returns true if the key was released this frame|
|GetMouseAim()|[Vector3](../static/vector3.md)|Returns the position the player is aiming at|
|GetCursorAimDirection()|[Vector3](../static/vector3.md)|Returns the ray the player is aiming at|
|GetMouseSpeed()|[Vector3](../static/vector3.md)|Returns the speed of the mouse|
|GetMousePosition()|[Vector3](../static/vector3.md)|Returns the position of the mouse|
|GetScreenDimensions()|[Vector3](../static/vector3.md)|Returns the dimensions of the screen|
|SetKeyDefaultEnabled(key : [String](../static/string.md), enabled : bool)|none|Sets whether the key is enabled by default|
|SetKeyHold(key : [String](../static/string.md), enabled : bool)|none|Sets whether the key is being held down|
