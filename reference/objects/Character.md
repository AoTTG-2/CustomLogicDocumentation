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
#### function <mark style="color:yellow;">GetKilled</mark>(killer: <mark style="color:blue;">[String](../static/String.md)</mark>) -> <mark style="color:blue;">void</mark>
> Kills the character. Callable by non-owners.

#### function <mark style="color:yellow;">GetDamaged</mark>(killer: <mark style="color:blue;">[String](../static/String.md)</mark>, damage: <mark style="color:blue;">int</mark>) -> <mark style="color:blue;">void</mark>
> Damages the character and kills it if its health reaches 0. Callable by non-owners.

#### function <mark style="color:yellow;">Emote</mark>(emote: <mark style="color:blue;">[String](../static/String.md)</mark>) -> <mark style="color:blue;">void</mark>
> Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.

#### function <mark style="color:yellow;">PlayAnimation</mark>(animation: <mark style="color:blue;">[String](../static/String.md)</mark>, fade: <mark style="color:blue;">float</mark> = <mark style="color:blue;">0.1</mark>) -> <mark style="color:blue;">void</mark>
> Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.

#### function <mark style="color:yellow;">ForceAnimation</mark>(animation: <mark style="color:blue;">[String](../static/String.md)</mark>, fade: <mark style="color:blue;">float</mark> = <mark style="color:blue;">0.1</mark>) -> <mark style="color:blue;">void</mark>
> Forces the character to play an animation. If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.

#### function <mark style="color:yellow;">GetAnimationLength</mark>(animation: <mark style="color:blue;">[String](../static/String.md)</mark>) -> <mark style="color:blue;">float</mark>
> Gets the length of animation.

#### function <mark style="color:yellow;">PlaySound</mark>(sound: <mark style="color:blue;">[String](../static/String.md)</mark>) -> <mark style="color:blue;">void</mark>
> Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.

#### function <mark style="color:yellow;">StopSound</mark>(sound: <mark style="color:blue;">[String](../static/String.md)</mark>) -> <mark style="color:blue;">void</mark>
> Stops the sound.

#### function <mark style="color:yellow;">LookAt</mark>(position: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>) -> <mark style="color:blue;">void</mark>
> Rotates the character such that it is looking towards a world position.

#### function <mark style="color:yellow;">AddForce</mark>(force: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>, mode: <mark style="color:blue;">[String](../static/String.md)</mark> = <mark style="color:blue;">Acceleration</mark>) -> <mark style="color:blue;">void</mark>
> Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.

#### function <mark style="color:yellow;">Reveal</mark>(delay: <mark style="color:blue;">float</mark>) -> <mark style="color:blue;">void</mark>
> Reveaal the titan for a set number of seconds.

#### function <mark style="color:yellow;">AddOutline</mark>(color: <mark style="color:blue;">[Color](../objects/Color.md)</mark> = <mark style="color:blue;">null</mark>, mode: <mark style="color:blue;">[String](../static/String.md)</mark> = <mark style="color:blue;">OutlineAll</mark>) -> <mark style="color:blue;">void</mark>
> Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor

#### function <mark style="color:yellow;">RemoveOutline</mark>() -> <mark style="color:blue;">void</mark>
> Removes the outline effect from the character.


---

