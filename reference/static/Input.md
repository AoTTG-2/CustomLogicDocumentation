# Input
Inherits from object
## Static Methods
|Function|Returns|Description|
|---|---|---|
|GetKeyName(<i>key</i> : [String](../static/String.md))|[String](../static/String.md)|Gets the key name the player assigned to the key setting|
|GetKeyHold(<i>key</i> : [String](../static/String.md))|bool|Returns true if the key is being held down|
|GetKeyDown(<i>key</i> : [String](../static/String.md))|bool|Returns true if the key was pressed down this frame|
|GetKeyUp(<i>key</i> : [String](../static/String.md))|bool|Returns true if the key was released this frame|
|GetMouseAim()|[Vector3](../objects/Vector3.md)|Returns the position the player is aiming at|
|GetCursorAimDirection()|[Vector3](../objects/Vector3.md)|Returns the ray the player is aiming at|
|GetMouseSpeed()|[Vector3](../objects/Vector3.md)|Returns the speed of the mouse|
|GetMousePosition()|[Vector3](../objects/Vector3.md)|Returns the position of the mouse|
|GetScreenDimensions()|[Vector3](../objects/Vector3.md)|Returns the dimensions of the screen|
|SetKeyDefaultEnabled(<br/><i>key</i> : [String](../static/String.md),<br/><i>enabled</i> : bool<br/>)|none|Sets whether the key is enabled by default|
|SetKeyHold(<br/><i>key</i> : [String](../static/String.md),<br/><i>enabled</i> : bool<br/>)|none|Sets whether the key is being held down|
