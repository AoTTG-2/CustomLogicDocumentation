# Character
Inherits from [Object](./Object.md)

Character is the base class that Human, Titan, and Shifter inherit from.
Only character owner can modify fields and call functions unless otherwise specified.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Name|string|False|Character's name.|
|Guild|string|False|Character's guild.|
|Player|[Player](./Player.md)|True|Player who owns this character.|
|IsAI|bool|True|Is this character AI?|
|ViewID|int|True|Network view ID of the character.|
|IsMine|bool|True|Is this character mine?|
|IsMainCharacter|bool|True|Character belongs to my player and is the main character (the camera-followed player).|
|Transform|[Transform](./Transform.md)|True|Unity transform of the character.|
|Position|[Vector3](./Vector3.md)|False|Position of the character.|
|Rotation|[Vector3](./Vector3.md)|False|Rotation of the character.|
|QuaternionRotation|[Quaternion](./Quaternion.md)|False|Quaternion rotation of the character.|
|Velocity|[Vector3](./Vector3.md)|False|Velocity of the character.|
|Forward|[Vector3](./Vector3.md)|False|Forward direction of the character.|
|Right|[Vector3](./Vector3.md)|False|Right direction of the character.|
|Up|[Vector3](./Vector3.md)|False|Up direction of the character.|
|HasTargetDirection|bool|True|If the character has a target direction it is turning towards.|
|TargetDirection|[Vector3](./Vector3.md)|True|The character's target direction.|
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
<pre class="language-typescript"><code class="lang-typescript">function PlayAnimation(animation: string, fade: float) -> null</code></pre>
> Causes the character to play an animation.  If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
<pre class="language-typescript"><code class="lang-typescript">function ForceAnimation(animation: string, fade: float) -> null</code></pre>
> Forces the character to play an animation. If the fade parameter is provided, will crossfade the animation by this timestep. Available animations can be found here: Human, Titan, Annie, Eren. Use the right-hand string value for the animation.
<pre class="language-typescript"><code class="lang-typescript">function GetAnimationLength(animation: string) -> float</code></pre>
> Gets the length of animation.
<pre class="language-typescript"><code class="lang-typescript">function PlaySound(sound: string) -> null</code></pre>
> Plays a sound if present in the character. Available sound names can be found here: Humans, Shifters, Titans. Note that shifters also have all titan sounds.
<pre class="language-typescript"><code class="lang-typescript">function StopSound(sound: string) -> null</code></pre>
> Stops the sound.
<pre class="language-typescript"><code class="lang-typescript">function LookAt(position: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> null</code></pre>
> Rotates the character such that it is looking towards a world position.
<pre class="language-typescript"><code class="lang-typescript">function AddForce(force: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, mode: string) -> null</code></pre>
> Adds a force to the character with given force vector and optional mode. Valid modes are Force, Acceleration, Impulse, VelocityChange with default being Acceleration.
<pre class="language-typescript"><code class="lang-typescript">function Reveal(delay: float) -> null</code></pre>
> Reveal the titan for a set number of seconds.
<pre class="language-typescript"><code class="lang-typescript">function AddOutline(color: <a data-footnote-ref href="#user-content-fn-4">Color</a>, mode: string) -> null</code></pre>
> Adds an outline effect with the given color and mode. Valid modes are: OutlineAll, OutlineVisible, OutlineHidden, OutlineAndSilhouette, SilhouetteOnly, OutlineAndLightenColor
<pre class="language-typescript"><code class="lang-typescript">function RemoveOutline() -> null</code></pre>
> Removes the outline effect from the character.

[^1]: [Camera](./Camera.md)
[^2]: [Character](./Character.md)
[^3]: [Collider](./Collider.md)
[^4]: [Collision](./Collision.md)
[^5]: [Color](./Color.md)
[^6]: [Convert](./Convert.md)
[^7]: [Cutscene](./Cutscene.md)
[^8]: [Dict](./Dict.md)
[^9]: [Game](./Game.md)
[^10]: [Human](./Human.md)
[^11]: [Input](./Input.md)
[^12]: [Json](./Json.md)
[^13]: [LineCastHitResult](./LineCastHitResult.md)
[^14]: [LineRenderer](./LineRenderer.md)
[^15]: [List](./List.md)
[^16]: [Map](./Map.md)
[^17]: [MapObject](./MapObject.md)
[^18]: [MapTargetable](./MapTargetable.md)
[^19]: [Math](./Math.md)
[^20]: [Network](./Network.md)
[^21]: [NetworkView](./NetworkView.md)
[^22]: [PersistentData](./PersistentData.md)
[^23]: [Physics](./Physics.md)
[^24]: [Player](./Player.md)
[^25]: [Quaternion](./Quaternion.md)
[^26]: [Random](./Random.md)
[^27]: [Range](./Range.md)
[^28]: [RoomData](./RoomData.md)
[^29]: [Set](./Set.md)
[^30]: [Shifter](./Shifter.md)
[^31]: [String](./String.md)
[^32]: [Time](./Time.md)
[^33]: [Titan](./Titan.md)
[^34]: [Transform](./Transform.md)
[^35]: [UI](./UI.md)
[^36]: [Vector2](./Vector2.md)
[^37]: [Vector3](./Vector3.md)
[^38]: [Object](./Object.md)
