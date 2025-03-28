# Titan
Inherits from [Character](../objects/Character.md)
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Name|[String](../static/String.md)|False|Titans's name.|
|Guild|[String](../static/String.md)|False|Titans's guild.|
|Size|float|False|Titan's size.|
|RunSpeedBase|float|False|Titan's base run speed. Final run speed is RunSpeedBase + Size * RunSpeedPerLevel.|
|WalkSpeedBase|float|False|Titan's base walk speed. Final walk speed is WalkSpeedBase + Size * WalkSpeedPerLevel.|
|WalkSpeedPerLevel|float|False|Titan's walk speed added per size.|
|RunSpeedPerLevel|float|False|Titan's run speed added per size.|
|TurnSpeed|float|False|Titan's turn animation speed.|
|RotateSpeed|float|False|Titan's rotate speed.|
|JumpForce|float|False|Titan's jump force.|
|ActionPause|float|False|Titan's pause delay after performing an action.|
|AttackPause|float|False|Titan's pause delay after performing an attack.|
|TurnPause|float|False|Titan's pause delay after performing a turn.|
|Stamina|float|False|PT stamina.|
|MaxStamina|float|False|PT max stamina.|
|NapePosition|[Vector3](../objects/Vector3.md)|False|The titan's nape position.|
|IsCrawler|bool|False|Is titan a crawler.|
|DetectRange|float|False|(AI) titan's detect range.|
|FocusRange|float|False|(AI) titan's focus range.|
|FocusTime|float|False|(AI) titan's focus time.|
|FarAttackCooldown|float|False|(AI) Titan's cooldown after performing a ranged attack.|
|AttackWait|float|False|(AI) Titan's wait time between being in range and performing an attack.|
|CanRun|bool|False|(AI) Titan can run or only walk.|
|AttackSpeedMultiplier|float|False|Titan's attack animation speed.|
|UsePathfinding|bool|False|Determines whether the (AI) titan uses pathfinding. (Smart Movement in titan settings)|
|HeadMount|[Transform](../objects/Transform.md)|False|Titan's head transform.|
|NeckMount|[Transform](../objects/Transform.md)|False|Titan's neck transform.|
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
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">MoveTo</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">range</mark>, <mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">ignoreEnemies</mark>)
Causes the (AI) titan to move towards a position and stopping when within specified range. If ignoreEnemies is true, will not engage enemies along the way.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Target</mark>(<mark style="color:#509cd4;">Object</mark> <mark style="color:#9cdcfe;">enemyObj</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">focus</mark>)
Causes the (AI) titan to target an enemy character or MapTargetable for focusTime seconds. If focusTime is 0 it will use the default focus time
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Idle</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">time</mark>)
Causes the (AI) titan to idle for time seconds before beginning to wander. During idle the titan will not react or move at all.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Wander</mark>()
Causes the (AI) titan to cancel any move commands and begin wandering randomly.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Blind</mark>()
Causes the titan to enter the blind state.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Cripple</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">time</mark>)
Causes the titan to enter the cripple state for time seconds. Using 0 will use the default cripple time.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">GetKilled</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">killer</mark>)
Kills the character. Callable by non-owners.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">GetDamaged</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">killer</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">damage</mark>)
Damages the character and kills it if its health reaches 0. Callable by non-owners.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Emote</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">emote</mark>)
Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">PlayAnimation</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">animation</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">fade</mark> = <mark style="color:#509cd4;">0.1</mark>)
Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ForceAnimation</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">animation</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">fade</mark> = <mark style="color:#509cd4;">0.1</mark>)
Forces the character to play an animation. If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">GetAnimationLength</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">animation</mark>)
Gets the length of animation.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">PlaySound</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">sound</mark>)
Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">StopSound</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">sound</mark>)
Stops the sound.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">LookAt</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">position</mark>)
Rotates the character such that it is looking towards a world position.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">AddForce</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">force</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">mode</mark> = <mark style="color:#509cd4;">Acceleration</mark>)
Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Reveal</mark>(<mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">delay</mark>)
Reveaal the titan for a set number of seconds.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">AddOutline</mark>(<mark style="color:#509cd4;">[Color](../objects/Color.md)</mark> <mark style="color:#9cdcfe;">color</mark> = <mark style="color:#509cd4;">null</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">mode</mark> = <mark style="color:#509cd4;">OutlineAll</mark>)
Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">RemoveOutline</mark>()
Removes the outline effect from the character.

---

