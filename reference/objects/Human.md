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
#### <span style="color:blue;">bool</span> <span style="color:yellow;">Refill</span>()
> Refills the gas of the human
#### <span style="color:blue;">void</span> <span style="color:yellow;">RefillImmediate</span>()
> Refills the gas of the human immediately
#### <span style="color:blue;">void</span> <span style="color:yellow;">ClearHooks</span>()
> Clears all hooks
#### <span style="color:blue;">void</span> <span style="color:yellow;">ClearLeftHook</span>()
> Clears the left hook
#### <span style="color:blue;">void</span> <span style="color:yellow;">ClearRightHook</span>()
> Clears the right hook
#### <span style="color:blue;">void</span> <span style="color:yellow;">MountMapObject</span>(<span style="color:blue;">[MapObject](../objects/MapObject.md)</span> mapObject, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> positionOffset, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> rotationOffset)
> Mounts the human on a map object
#### <span style="color:blue;">void</span> <span style="color:yellow;">MountTransform</span>(<span style="color:blue;">[Transform](../objects/Transform.md)</span> transform, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> positionOffset, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> rotationOffset)
> Mounts the human on a transform
#### <span style="color:blue;">void</span> <span style="color:yellow;">Unmount</span>()
> Unmounts the human
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetSpecial</span>(<span style="color:blue;">[String](../static/String.md)</span> special)
> Sets the special of the human
#### <span style="color:blue;">void</span> <span style="color:yellow;">ActivateSpecial</span>()
> Activates the special of the human
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetWeapon</span>(<span style="color:blue;">[String](../static/String.md)</span> weapon)
> Sets the weapon of the human
#### <span style="color:blue;">void</span> <span style="color:yellow;">DisablePerks</span>()
> Disables all perks of the human
#### <span style="color:blue;">void</span> <span style="color:yellow;">GetKilled</span>(<span style="color:blue;">[String](../static/String.md)</span> killer)
> Kills the character. Callable by non-owners.
#### <span style="color:blue;">void</span> <span style="color:yellow;">GetDamaged</span>(<span style="color:blue;">[String](../static/String.md)</span> killer, <span style="color:blue;">int</span> damage)
> Damages the character and kills it if its health reaches 0. Callable by non-owners.
#### <span style="color:blue;">void</span> <span style="color:yellow;">Emote</span>(<span style="color:blue;">[String](../static/String.md)</span> emote)
> Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.
#### <span style="color:blue;">void</span> <span style="color:yellow;">PlayAnimation</span>(<span style="color:blue;">[String](../static/String.md)</span> animation, <span style="color:blue;">float</span> fade = <span style="color:blue;">0.1</span>)
> Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <span style="color:blue;">void</span> <span style="color:yellow;">ForceAnimation</span>(<span style="color:blue;">[String](../static/String.md)</span> animation, <span style="color:blue;">float</span> fade = <span style="color:blue;">0.1</span>)
> Forces the character to play an animation. If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <span style="color:blue;">float</span> <span style="color:yellow;">GetAnimationLength</span>(<span style="color:blue;">[String](../static/String.md)</span> animation)
> Gets the length of animation.
#### <span style="color:blue;">void</span> <span style="color:yellow;">PlaySound</span>(<span style="color:blue;">[String](../static/String.md)</span> sound)
> Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.
#### <span style="color:blue;">void</span> <span style="color:yellow;">StopSound</span>(<span style="color:blue;">[String](../static/String.md)</span> sound)
> Stops the sound.
#### <span style="color:blue;">void</span> <span style="color:yellow;">LookAt</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> position)
> Rotates the character such that it is looking towards a world position.
#### <span style="color:blue;">void</span> <span style="color:yellow;">AddForce</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> force, <span style="color:blue;">[String](../static/String.md)</span> mode = <span style="color:blue;">Acceleration</span>)
> Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.
#### <span style="color:blue;">void</span> <span style="color:yellow;">Reveal</span>(<span style="color:blue;">float</span> delay)
> Reveaal the titan for a set number of seconds.
#### <span style="color:blue;">void</span> <span style="color:yellow;">AddOutline</span>(<span style="color:blue;">[Color](../objects/Color.md)</span> color = <span style="color:blue;">null</span>, <span style="color:blue;">[String](../static/String.md)</span> mode = <span style="color:blue;">OutlineAll</span>)
> Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor
#### <span style="color:blue;">void</span> <span style="color:yellow;">RemoveOutline</span>()
> Removes the outline effect from the character.

---

