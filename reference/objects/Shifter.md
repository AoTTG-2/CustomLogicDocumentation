# Shifter
Inherits from [Character](../objects/Character.md)
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Name|[String](../static/String.md)|False|Shifter's name.|
|Guild|[String](../static/String.md)|False|Shifter's guild.|
|Size|float|False|Shifter's size.|
|RunSpeedBase|float|False|Shifter's base run speed. Final run speed is RunSpeedBase + Size * RunSpeedPerLevel.|
|WalkSpeedBase|float|False|Shifter's base walk speed. Final walk speed is WalkSpeedBase + Size * WalkSpeedPerLevel.|
|WalkSpeedPerLevel|float|False|Shifter's walk speed added per level.|
|RunSpeedPerLevel|float|False|Shifter's run speed added per level.|
|TurnSpeed|float|False|Shifter's turn speed when running turn animation.|
|RotateSpeed|float|False|Shifter's rotate speed when rotating body.|
|JumpForce|float|False|Shifter's jump force when jumping.|
|ActionPause|float|False|Shifter's pause delay after performing an action.|
|AttackPause|float|False|Shifter's pause delay after performing an attack.|
|TurnPause|float|False|Shifter's pause delay after performing a turn.|
|DetectRange|float|False|(AI) shifter's detect range.|
|FocusRange|float|False|(AI) shifter's focus range.|
|FocusTime|float|False|(AI) shifter's focus time before switching targets.|
|FarAttackCooldown|float|False|(AI) Shifter's cooldown after performing a ranged attack.|
|AttackWait|float|False|(AI) Shifter's wait time between being in range to attack and performing the attack.|
|AttackSpeedMultiplier|float|False|Shifter's attack animation speed.|
|UsePathfinding|bool|False|(AI) Shifter uses pathfinding.|
|NapePosition|[Vector3](../objects/Vector3.md)|False|The shifter's nape position.|
|DeathAnimLength|float|False|The length of the death animation.|
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
#### void <span style="color":#dcdcaa>MoveTo<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>, float <span style="color":#9cdcfe>range<span>, bool <span style="color":#9cdcfe>ignoreEnemies<span>)
Causes the (AI) shifter to move towards a position. If ignoreEnemies is true, will not engage enemies along the way.
#### void <span style="color":#dcdcaa>Target<span>(Object <span style="color":#9cdcfe>enemyObj<span>, float <span style="color":#9cdcfe>focus<span>)
Causes the (AI) shifter to target an enemy character or MapTargetable for focusTime seconds. If focusTime is 0 it will use the default focus time.
#### void <span style="color":#dcdcaa>Idle<span>(float <span style="color":#9cdcfe>time<span>)
Causes the (AI) shifter to idle for time seconds before beginning to wander. During idle the titan will not react or move at all.
#### void <span style="color":#dcdcaa>Wander<span>()
Causes the (AI) shifter to cancel any move commands and begin wandering randomly.
#### void <span style="color":#dcdcaa>Blind<span>()
Causes the shifter to enter the blind state.
#### void <span style="color":#dcdcaa>Cripple<span>(float <span style="color":#9cdcfe>time<span>)
Causes the shifter to enter the cripple state.
#### void <span style="color":#dcdcaa>GetKilled<span>([String](../static/String.md) <span style="color":#9cdcfe>killer<span>)
Kills the character. Callable by non-owners.
#### void <span style="color":#dcdcaa>GetDamaged<span>([String](../static/String.md) <span style="color":#9cdcfe>killer<span>, int <span style="color":#9cdcfe>damage<span>)
Damages the character and kills it if its health reaches 0. Callable by non-owners.
#### void <span style="color":#dcdcaa>Emote<span>([String](../static/String.md) <span style="color":#9cdcfe>emote<span>)
Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.
#### void <span style="color":#dcdcaa>PlayAnimation<span>([String](../static/String.md) <span style="color":#9cdcfe>animation<span>, float <span style="color":#9cdcfe>fade<span> = 0.1)
Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### void <span style="color":#dcdcaa>ForceAnimation<span>([String](../static/String.md) <span style="color":#9cdcfe>animation<span>, float <span style="color":#9cdcfe>fade<span> = 0.1)
Forces the character to play an animation. If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### float <span style="color":#dcdcaa>GetAnimationLength<span>([String](../static/String.md) <span style="color":#9cdcfe>animation<span>)
Gets the length of animation.
#### void <span style="color":#dcdcaa>PlaySound<span>([String](../static/String.md) <span style="color":#9cdcfe>sound<span>)
Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.
#### void <span style="color":#dcdcaa>StopSound<span>([String](../static/String.md) <span style="color":#9cdcfe>sound<span>)
Stops the sound.
#### void <span style="color":#dcdcaa>LookAt<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>position<span>)
Rotates the character such that it is looking towards a world position.
#### void <span style="color":#dcdcaa>AddForce<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>force<span>, [String](../static/String.md) <span style="color":#9cdcfe>mode<span> = Acceleration)
Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.
#### void <span style="color":#dcdcaa>Reveal<span>(float <span style="color":#9cdcfe>delay<span>)
Reveaal the titan for a set number of seconds.
#### void <span style="color":#dcdcaa>AddOutline<span>([Color](../objects/Color.md) <span style="color":#9cdcfe>color<span> = null, [String](../static/String.md) <span style="color":#9cdcfe>mode<span> = OutlineAll)
Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor
#### void <span style="color":#dcdcaa>RemoveOutline<span>()
Removes the outline effect from the character.

---

