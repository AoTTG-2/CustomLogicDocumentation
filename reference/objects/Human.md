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
#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">Refill</mark>()
Refills the gas of the human
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">RefillImmediate</mark>()
Refills the gas of the human immediately
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ClearHooks</mark>()
Clears all hooks
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ClearLeftHook</mark>()
Clears the left hook
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ClearRightHook</mark>()
Clears the right hook
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">MountMapObject</mark>(<mark style="color:blue;">[MapObject](../objects/MapObject.md)</mark> <mark style="color:yellow;">mapObject</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">positionOffset</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">rotationOffset</mark>)
Mounts the human on a map object
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">MountTransform</mark>(<mark style="color:blue;">[Transform](../objects/Transform.md)</mark> <mark style="color:yellow;">transform</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">positionOffset</mark>, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">rotationOffset</mark>)
Mounts the human on a transform
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Unmount</mark>()
Unmounts the human
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetSpecial</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">special</mark>)
Sets the special of the human
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ActivateSpecial</mark>()
Activates the special of the human
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetWeapon</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">weapon</mark>)
Sets the weapon of the human
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">DisablePerks</mark>()
Disables all perks of the human
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">GetKilled</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">killer</mark>)
Kills the character. Callable by non-owners.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">GetDamaged</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">killer</mark>, <mark style="color:blue;">int</mark> <mark style="color:yellow;">damage</mark>)
Damages the character and kills it if its health reaches 0. Callable by non-owners.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Emote</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">emote</mark>)
Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">PlayAnimation</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">animation</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">fade</mark> = <mark style="color:blue;">0.1</mark>)
Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ForceAnimation</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">animation</mark>, <mark style="color:blue;">float</mark> <mark style="color:yellow;">fade</mark> = <mark style="color:blue;">0.1</mark>)
Forces the character to play an animation. If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">GetAnimationLength</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">animation</mark>)
Gets the length of animation.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">PlaySound</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">sound</mark>)
Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">StopSound</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">sound</mark>)
Stops the sound.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">LookAt</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">position</mark>)
Rotates the character such that it is looking towards a world position.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">AddForce</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">force</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">mode</mark> = <mark style="color:blue;">Acceleration</mark>)
Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Reveal</mark>(<mark style="color:blue;">float</mark> <mark style="color:yellow;">delay</mark>)
Reveaal the titan for a set number of seconds.
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">AddOutline</mark>(<mark style="color:blue;">[Color](../objects/Color.md)</mark> <mark style="color:yellow;">color</mark> = <mark style="color:blue;">null</mark>, <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">mode</mark> = <mark style="color:blue;">OutlineAll</mark>)
Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">RemoveOutline</mark>()
Removes the outline effect from the character.

---

