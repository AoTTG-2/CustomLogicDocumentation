# Character
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Name|[String](../static/String.md)|False|Character's name.|
|Guild|[String](../static/String.md)|False|Character's guild.|
|Player|[Player](../objects/Player.md)|False|Player who owns this character.|
|IsAI|bool|False|Is this character AI?|
|ViewID|int|False|Network view ID of the character.|
|IsMine|bool|False|Is this character mine?|
|IsMainCharacter|bool|False||
|Transform|[Transform](../objects/Transform.md)|False|Unity transform of the character.|
|Position|[Vector3](../objects/Vector3.md)|False|Position of the character.|
|Rotation|[Vector3](../objects/Vector3.md)|False|Rotation of the character.|
|QuaternionRotation|[Quaternion](../objects/Quaternion.md)|False|Quaternion rotation of the character.|
|Velocity|[Vector3](../objects/Vector3.md)|False|Velocity of the character.|
|Forward|[Vector3](../objects/Vector3.md)|False|Forward direction of the character.|
|Right|[Vector3](../objects/Vector3.md)|False|Right direction of the character.|
|Up|[Vector3](../objects/Vector3.md)|False|Up direction of the character.|
|HasTargetDirection|bool|False|If the character has a target direction it is turning towards.|
|TargetDirection|[Vector3](../objects/Vector3.md)|False|The character's target direction.|
|Team|[String](../static/String.md)|False|Team character belongs to.|
|Health|float|False|Character's current health.|
|MaxHealth|float|False|Character's maximum health.|
|CustomDamageEnabled|bool|False|Is custom damage dealing enabled.|
|CustomDamage|int|False|Amount of custom damage to deal per attack.|
|CurrentAnimation|[String](../static/String.md)|False|Character's current playing animation.|
|Grounded|bool|False|Character's grounded status.|
## Methods
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">GetKilled</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">killer</span>)
Kills the character. Callable by non-owners.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">GetDamaged</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">killer</span>, <span style="color:#509cd4;">int</span> <span style="color:#9cdcfe;">damage</span>)
Damages the character and kills it if its health reaches 0. Callable by non-owners.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Emote</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">emote</span>)
Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">PlayAnimation</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">animation</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">fade</span> = <span style="color:#509cd4;">0.1</span>)
Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">ForceAnimation</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">animation</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">fade</span> = <span style="color:#509cd4;">0.1</span>)
Forces the character to play an animation. If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <span style="color:#509cd4;">float</span> <span style="color:#dcdcaa;">GetAnimationLength</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">animation</span>)
Gets the length of animation.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">PlaySound</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">sound</span>)
Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">StopSound</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">sound</span>)
Stops the sound.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">LookAt</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">position</span>)
Rotates the character such that it is looking towards a world position.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">AddForce</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">force</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">mode</span> = <span style="color:#509cd4;">Acceleration</span>)
Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Reveal</span>(<span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">delay</span>)
Reveaal the titan for a set number of seconds.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">AddOutline</span>(<span style="color:#509cd4;">[Color](../objects/Color.md)</span> <span style="color:#9cdcfe;">color</span> = <span style="color:#509cd4;">null</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">mode</span> = <span style="color:#509cd4;">OutlineAll</span>)
Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">RemoveOutline</span>()
Removes the outline effect from the character.

---

