# Human
Inherits from [Character](../objects/Character.md)
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Name|[String](../static/String.md)|False|The human's name|
|Guild|[String](../static/String.md)|False|The human's guild|
|Weapon|[String](../static/String.md)|False|The weapon the human is using|
|CurrentSpecial|[String](../static/String.md)|False|The current special the human is using|
|SpecialCooldown|float|False|The cooldown of the special|
|ShifterLiveTime|float|False|The live time of the shifter special|
|SpecialCooldownRatio|float|False|The ratio of the special cooldown|
|CurrentGas|float|False|The current gas of the human|
|MaxGas|float|False|The max gas of the human|
|Acceleration|int|False|The acceleration of the human|
|Speed|int|False|The speed of the human|
|HorseSpeed|float|False|The speed of the horse|
|CurrentBladeDurability|float|False|The current blade durability|
|MaxBladeDurability|float|False|The max blade durability|
|CurrentBlade|int|False|The current blade|
|MaxBlade|int|False|The max number of blades held|
|CurrentAmmoRound|int|False|The current ammo round|
|MaxAmmoRound|int|False|The max ammo round|
|CurrentAmmoLeft|int|False|The current ammo left|
|MaxAmmoTotal|int|False|The max total ammo|
|LeftHookEnabled|bool|False|Whether the left hook is enabled|
|RightHookEnabled|bool|False|Whether the right hook is enabled|
|IsMounted|bool|False|Whether the human is mounted|
|MountedMapObject|[MapObject](../objects/MapObject.md)|False|The map object the human is mounted on|
|MountedTransform|[Transform](../objects/Transform.md)|False|The transform the human is mounted on|
|AutoRefillGas|bool|False|Whether the human auto refills gas|
|State|[String](../static/String.md)|False|The state of the human|
|CanDodge|bool|False|Whether the human can dodge|
|IsInvincible|bool|False|Whether the human is invincible|
|InvincibleTimeLeft|float|False|The time left for invincibility|
|IsCarried|bool|False|If the human is carried.|
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
|Function|Returns|Description|
|---|---|---|
|Refill()|bool|Refills the gas of the human|
|RefillImmediate()|none|Refills the gas of the human immediately|
|ClearHooks()|none|Clears all hooks|
|ClearLeftHook()|none|Clears the left hook|
|ClearRightHook()|none|Clears the right hook|
|MountMapObject(<br/>mapObject : [MapObject](../objects/MapObject.md),<br/>positionOffset : [Vector3](../objects/Vector3.md),<br/>rotationOffset : [Vector3](../objects/Vector3.md)<br/>)|none|Mounts the human on a map object|
|MountTransform(<br/>transform : [Transform](../objects/Transform.md),<br/>positionOffset : [Vector3](../objects/Vector3.md),<br/>rotationOffset : [Vector3](../objects/Vector3.md)<br/>)|none|Mounts the human on a transform|
|Unmount()|none|Unmounts the human|
|SetSpecial(special : [String](../static/String.md))|none|Sets the special of the human|
|ActivateSpecial()|none|Activates the special of the human|
|SetWeapon(weapon : [String](../static/String.md))|none|Sets the weapon of the human|
|DisablePerks()|none|Disables all perks of the human|
|GetKilled(killer : [String](../static/String.md))|none|Kills the character. Callable by non-owners.|
|GetDamaged(<br/>killer : [String](../static/String.md),<br/>damage : int<br/>)|none|Damages the character and kills it if its health reaches 0. Callable by non-owners.|
|Emote(emote : [String](../static/String.md))|none|Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.|
|PlayAnimation(<br/>animation : [String](../static/String.md),<br/>fade : float = 0.1<br/>)|none|Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.|
|GetAnimationLength(animation : [String](../static/String.md))|float|Gets the length of animation.|
|PlaySound(sound : [String](../static/String.md))|none|Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.|
|StopSound(sound : [String](../static/String.md))|none|Stops the sound.|
|LookAt(position : [Vector3](../objects/Vector3.md))|none|Rotates the character such that it is looking towards a world position.|
|AddForce(<br/>force : [Vector3](../objects/Vector3.md),<br/>mode : [String](../static/String.md) = Acceleration<br/>)|none|Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.|
|Reveal(delay : float)|none|Reveaal the titan for a set number of seconds.|
|AddOutline(<br/>color : [Color](../objects/Color.md) = ,<br/>mode : [String](../static/String.md) = OutlineAll<br/>)|none|Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor|
|RemoveOutline()|none|Removes the outline effect from the character.|
