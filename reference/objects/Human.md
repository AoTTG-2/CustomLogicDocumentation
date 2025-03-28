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
#### <span style="color:#509cd4">bool</span> <span style="color:#dcdcaa">Refill</span>()
Refills the gas of the human
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">RefillImmediate</span>()
Refills the gas of the human immediately
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">ClearHooks</span>()
Clears all hooks
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">ClearLeftHook</span>()
Clears the left hook
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">ClearRightHook</span>()
Clears the right hook
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">MountMapObject</span>(<span style="color:#509cd4">[MapObject](../objects/MapObject.md)</span> <span style="color:#9cdcfe">mapObject</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">positionOffset</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">rotationOffset</span>)
Mounts the human on a map object
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">MountTransform</span>(<span style="color:#509cd4">[Transform](../objects/Transform.md)</span> <span style="color:#9cdcfe">transform</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">positionOffset</span>, <span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">rotationOffset</span>)
Mounts the human on a transform
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Unmount</span>()
Unmounts the human
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SetSpecial</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">special</span>)
Sets the special of the human
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">ActivateSpecial</span>()
Activates the special of the human
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">SetWeapon</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">weapon</span>)
Sets the weapon of the human
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">DisablePerks</span>()
Disables all perks of the human
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">GetKilled</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">killer</span>)
Kills the character. Callable by non-owners.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">GetDamaged</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">killer</span>, <span style="color:#509cd4">int</span> <span style="color:#9cdcfe">damage</span>)
Damages the character and kills it if its health reaches 0. Callable by non-owners.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Emote</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">emote</span>)
Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">PlayAnimation</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">animation</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">fade</span> = <span style="color:#509cd4">0.1</span>)
Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">ForceAnimation</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">animation</span>, <span style="color:#509cd4">float</span> <span style="color:#9cdcfe">fade</span> = <span style="color:#509cd4">0.1</span>)
Forces the character to play an animation. If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
#### <span style="color:#509cd4">float</span> <span style="color:#dcdcaa">GetAnimationLength</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">animation</span>)
Gets the length of animation.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">PlaySound</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">sound</span>)
Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">StopSound</span>(<span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">sound</span>)
Stops the sound.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">LookAt</span>(<span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">position</span>)
Rotates the character such that it is looking towards a world position.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">AddForce</span>(<span style="color:#509cd4">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe">force</span>, <span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">mode</span> = <span style="color:#509cd4">Acceleration</span>)
Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">Reveal</span>(<span style="color:#509cd4">float</span> <span style="color:#9cdcfe">delay</span>)
Reveaal the titan for a set number of seconds.
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">AddOutline</span>(<span style="color:#509cd4">[Color](../objects/Color.md)</span> <span style="color:#9cdcfe">color</span> = <span style="color:#509cd4">null</span>, <span style="color:#509cd4">[String](../static/String.md)</span> <span style="color:#9cdcfe">mode</span> = <span style="color:#509cd4">OutlineAll</span>)
Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor
#### <span style="color:#509cd4">void</span> <span style="color:#dcdcaa">RemoveOutline</span>()
Removes the outline effect from the character.

---

