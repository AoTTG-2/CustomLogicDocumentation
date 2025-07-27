# Human
Inherits from [Character](../md/objects/Character.md)
### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Name|string|False|The human's name|
|Guild|string|False|The human's guild|
|Weapon|string|False|The weapon the human is using|
|CurrentSpecial|string|False|The current special the human is using|
|SpecialCooldown|float|False|The cooldown of the special|
|ShifterLiveTime|float|False|The live time of the shifter special|
|SpecialCooldownRatio|float|True|The ratio of the special cooldown|
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
|IsMounted|bool|True|Whether the human is mounted|
|MountedMapObject|[MapObject](../md/objects/MapObject.md)|True|The map object the human is mounted on|
|MountedTransform|[Transform](../md/objects/Transform.md)|True|The transform the human is mounted on|
|AutoRefillGas|bool|False|Whether the human auto refills gas|
|State|string|True|The state of the human|
|CanDodge|bool|False|Whether the human can dodge|
|IsInvincible|bool|False|Whether the human is invincible|
|InvincibleTimeLeft|float|False|The time left for invincibility|
|IsCarried|bool|True|If the human is carried.|
|Player|[Player](../md/objects/Player.md)|True|Player who owns this character.|
|IsAI|bool|True|Is this character AI?|
|ViewID|int|True|Network view ID of the character.|
|IsMine|bool|True|Is this character mine?|
|IsMainCharacter|bool|True|Character belongs to my player and is the main character (the camera-followed player).|
|Transform|[Transform](../md/objects/Transform.md)|True|Unity transform of the character.|
|Position|[Vector3](../md/objects/Vector3.md)|False|Position of the character.|
|Rotation|[Vector3](../md/objects/Vector3.md)|False|Rotation of the character.|
|QuaternionRotation|[Quaternion](../md/objects/Quaternion.md)|False|Quaternion rotation of the character.|
|Velocity|[Vector3](../md/objects/Vector3.md)|False|Velocity of the character.|
|Forward|[Vector3](../md/objects/Vector3.md)|False|Forward direction of the character.|
|Right|[Vector3](../md/objects/Vector3.md)|False|Right direction of the character.|
|Up|[Vector3](../md/objects/Vector3.md)|False|Up direction of the character.|
|HasTargetDirection|bool|True|If the character has a target direction it is turning towards.|
|TargetDirection|[Vector3](../md/objects/Vector3.md)|True|The character's target direction.|
|Team|string|False|Team character belongs to.|
|Health|float|False|Character's current health.|
|MaxHealth|float|False|Character's maximum health.|
|CustomDamageEnabled|bool|False|Is custom damage dealing enabled.|
|CustomDamage|int|False|Amount of custom damage to deal per attack.|
|CurrentAnimation|string|True|Character's current playing animation.|
|Grounded|bool|True|Character's grounded status.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Refill() -> bool</code></pre>
> Refills the gas of the human

<pre class="language-typescript"><code class="lang-typescript">function RefillImmediate() -> null</code></pre>
> Refills the gas of the human immediately

<pre class="language-typescript"><code class="lang-typescript">function ClearHooks() -> null</code></pre>
> Clears all hooks

<pre class="language-typescript"><code class="lang-typescript">function ClearLeftHook() -> null</code></pre>
> Clears the left hook

<pre class="language-typescript"><code class="lang-typescript">function ClearRightHook() -> null</code></pre>
> Clears the right hook

<pre class="language-typescript"><code class="lang-typescript">function MountMapObject(mapObject: <a data-footnote-ref href="#user-content-fn-MapObject">MapObject</a>, positionOffset: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, rotationOffset: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [canMountedAttack: bool = False]) -> null</code></pre>
> Mounts the human on a map object

<pre class="language-typescript"><code class="lang-typescript">function MountTransform(transform: <a data-footnote-ref href="#user-content-fn-Transform">Transform</a>, positionOffset: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, rotationOffset: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [canMountedAttack: bool = False]) -> null</code></pre>
> Mounts the human on a transform

<pre class="language-typescript"><code class="lang-typescript">function Unmount([immediate: bool = True]) -> null</code></pre>
> Unmounts the human

<pre class="language-typescript"><code class="lang-typescript">function SetSpecial(special: string) -> null</code></pre>
> Sets the special of the human

<pre class="language-typescript"><code class="lang-typescript">function ActivateSpecial() -> null</code></pre>
> Activates the special of the human

<pre class="language-typescript"><code class="lang-typescript">function SetWeapon(weapon: string) -> null</code></pre>
> Sets the weapon of the human

<pre class="language-typescript"><code class="lang-typescript">function DisablePerks() -> null</code></pre>
> Disables all perks of the human

<pre class="language-typescript"><code class="lang-typescript">function GetKilled(killer: string) -> null</code></pre>
> Kills the character. Callable by non-owners.

<pre class="language-typescript"><code class="lang-typescript">function GetDamaged(killer: string, damage: int) -> null</code></pre>
> Damages the character and kills it if its health reaches 0. Callable by non-owners.

<pre class="language-typescript"><code class="lang-typescript">function Emote(emote: string) -> null</code></pre>
> Causes the character to emote. The list of available emotes is the same as those shown in the in-game emote menu.

<pre class="language-typescript"><code class="lang-typescript">function PlayAnimation(animation: string, [fade: float = 0.1]) -> null</code></pre>
> Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.

<pre class="language-typescript"><code class="lang-typescript">function ForceAnimation(animation: string, [fade: float = 0.1]) -> null</code></pre>
> Forces the character to play an animation. If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.

<pre class="language-typescript"><code class="lang-typescript">function GetAnimationLength(animation: string) -> float</code></pre>
> Gets the length of animation.

<pre class="language-typescript"><code class="lang-typescript">function PlaySound(sound: string) -> null</code></pre>
> Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.

<pre class="language-typescript"><code class="lang-typescript">function StopSound(sound: string) -> null</code></pre>
> Stops the sound.

<pre class="language-typescript"><code class="lang-typescript">function LookAt(position: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>) -> null</code></pre>
> Rotates the character such that it is looking towards a world position.

<pre class="language-typescript"><code class="lang-typescript">function AddForce(force: <a data-footnote-ref href="#user-content-fn-Vector3">Vector3</a>, [mode: string = Acceleration]) -> null</code></pre>
> Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.

<pre class="language-typescript"><code class="lang-typescript">function Reveal(delay: float) -> null</code></pre>
> Reveal the titan for a set number of seconds.

<pre class="language-typescript"><code class="lang-typescript">function AddOutline([color: <a data-footnote-ref href="#user-content-fn-Color">Color</a> = null], [mode: string = OutlineAll]) -> null</code></pre>
> Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor

<pre class="language-typescript"><code class="lang-typescript">function RemoveOutline() -> null</code></pre>
> Removes the outline effect from the character.


[^Camera]: [Camera](../md/static/Camera.md)
[^Character]: [Character](../md/objects/Character.md)
[^Collider]: [Collider](../md/objects/Collider.md)
[^Collision]: [Collision](../md/objects/Collision.md)
[^Color]: [Color](../md/objects/Color.md)
[^Convert]: [Convert](../md/static/Convert.md)
[^Cutscene]: [Cutscene](../md/static/Cutscene.md)
[^Dict]: [Dict](../md/objects/Dict.md)
[^Game]: [Game](../md/static/Game.md)
[^Human]: [Human](../md/objects/Human.md)
[^Input]: [Input](../md/static/Input.md)
[^Json]: [Json](../md/static/Json.md)
[^LineCastHitResult]: [LineCastHitResult](../md/objects/LineCastHitResult.md)
[^LineRenderer]: [LineRenderer](../md/objects/LineRenderer.md)
[^List]: [List](../md/objects/List.md)
[^Map]: [Map](../md/static/Map.md)
[^MapObject]: [MapObject](../md/objects/MapObject.md)
[^MapTargetable]: [MapTargetable](../md/objects/MapTargetable.md)
[^Math]: [Math](../md/static/Math.md)
[^Network]: [Network](../md/static/Network.md)
[^NetworkView]: [NetworkView](../md/objects/NetworkView.md)
[^PersistentData]: [PersistentData](../md/static/PersistentData.md)
[^Physics]: [Physics](../md/static/Physics.md)
[^Player]: [Player](../md/objects/Player.md)
[^Quaternion]: [Quaternion](../md/objects/Quaternion.md)
[^Random]: [Random](../md/objects/Random.md)
[^Range]: [Range](../md/objects/Range.md)
[^RoomData]: [RoomData](../md/static/RoomData.md)
[^Set]: [Set](../md/objects/Set.md)
[^Shifter]: [Shifter](../md/objects/Shifter.md)
[^String]: [String](../md/static/String.md)
[^Time]: [Time](../md/static/Time.md)
[^Titan]: [Titan](../md/objects/Titan.md)
[^Transform]: [Transform](../md/objects/Transform.md)
[^UI]: [UI](../md/static/UI.md)
[^Vector2]: [Vector2](../md/objects/Vector2.md)
[^Vector3]: [Vector3](../md/objects/Vector3.md)
[^Object]: [Object](../md/objects/Object.md)
[^Component]: [Component](../md/objects/Component.md)
