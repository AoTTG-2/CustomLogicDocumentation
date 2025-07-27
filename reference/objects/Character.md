# Character
Inherits from [Object](../md/objects/Object.md)

Character is the base class that Human, Titan, and Shifter inherit from.
Only character owner can modify fields and call functions unless otherwise specified.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Name|string|False|Character's name.|
|Guild|string|False|Character's guild.|
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
