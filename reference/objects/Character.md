# Character
Inherits from [Object](../objects/Object.md)

Character is the base class that Human, Titan, and Shifter inherit from.
Only character owner can modify fields and call functions unless otherwise specified.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Name|string|False|Character's name.|
|Guild|string|False|Character's guild.|
|Player|[Player](../objects/Player.md)|True|Player who owns this character.|
|IsAI|bool|True|Is this character AI?|
|ViewID|int|True|Network view ID of the character.|
|IsMine|bool|True|Is this character mine?|
|IsMainCharacter|bool|True|Character belongs to my player and is the main character (the camera-followed player).|
|Transform|[Transform](../objects/Transform.md)|True|Unity transform of the character.|
|Position|[Vector3](../objects/Vector3.md)|False|Position of the character.|
|Rotation|[Vector3](../objects/Vector3.md)|False|Rotation of the character.|
|QuaternionRotation|[Quaternion](../objects/Quaternion.md)|False|Quaternion rotation of the character.|
|Velocity|[Vector3](../objects/Vector3.md)|False|Velocity of the character.|
|Forward|[Vector3](../objects/Vector3.md)|False|Forward direction of the character.|
|Right|[Vector3](../objects/Vector3.md)|False|Right direction of the character.|
|Up|[Vector3](../objects/Vector3.md)|False|Up direction of the character.|
|HasTargetDirection|bool|True|If the character has a target direction it is turning towards.|
|TargetDirection|[Vector3](../objects/Vector3.md)|True|The character's target direction.|
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


[^Camera]: [Camera](../static/Camera.md)
[^Character]: [Character](../objects/Character.md)
[^Collider]: [Collider](../objects/Collider.md)
[^Collision]: [Collision](../objects/Collision.md)
[^Color]: [Color](../objects/Color.md)
[^Convert]: [Convert](../static/Convert.md)
[^Cutscene]: [Cutscene](../static/Cutscene.md)
[^Dict]: [Dict](../objects/Dict.md)
[^Game]: [Game](../static/Game.md)
[^Human]: [Human](../objects/Human.md)
[^Input]: [Input](../static/Input.md)
[^Json]: [Json](../static/Json.md)
[^LineCastHitResult]: [LineCastHitResult](../objects/LineCastHitResult.md)
[^LineRenderer]: [LineRenderer](../objects/LineRenderer.md)
[^List]: [List](../objects/List.md)
[^Map]: [Map](../static/Map.md)
[^MapObject]: [MapObject](../objects/MapObject.md)
[^MapTargetable]: [MapTargetable](../objects/MapTargetable.md)
[^Math]: [Math](../static/Math.md)
[^Network]: [Network](../static/Network.md)
[^NetworkView]: [NetworkView](../objects/NetworkView.md)
[^PersistentData]: [PersistentData](../static/PersistentData.md)
[^Physics]: [Physics](../static/Physics.md)
[^Player]: [Player](../objects/Player.md)
[^Quaternion]: [Quaternion](../objects/Quaternion.md)
[^Random]: [Random](../objects/Random.md)
[^Range]: [Range](../objects/Range.md)
[^RoomData]: [RoomData](../static/RoomData.md)
[^Set]: [Set](../objects/Set.md)
[^Shifter]: [Shifter](../objects/Shifter.md)
[^String]: [String](../static/String.md)
[^Time]: [Time](../static/Time.md)
[^Titan]: [Titan](../objects/Titan.md)
[^Transform]: [Transform](../objects/Transform.md)
[^UI]: [UI](../static/UI.md)
[^Vector2]: [Vector2](../objects/Vector2.md)
[^Vector3]: [Vector3](../objects/Vector3.md)
[^Object]: [Object](../objects/Object.md)
[^Component]: [Component](../objects/Component.md)
