# Physics
Inherits from [Object](../objects/Object.md)

Static Physics class. Contains some common physics functions.

### Example
```csharp
start = Vector3(0);
end = Vector3(10);
# Options: All, MapObjects, Characters, Titans, Humans, Projectiles, Entities, Hitboxes, MapEditor
result = Physics.LineCast(start, end, "Entities");
Game.Print(result.IsCharacter);
Game.Print(result.IsMapObject);
Game.Print(result.Point);
Game.Print(result.Normal);
Game.Print(result.Distance);
Game.Print(result.Collider);
```
### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function GetPhysicsLayerMask(layers: <a data-footnote-ref href="#user-content-fn-3">List</a>) -> int</code></pre>
> Get a physics layer mask with several layer id.
> 
<pre class="language-typescript"><code class="lang-typescript">function LineCast(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-2">LineCastHitResult</a></code></pre>
> Performs a line cast between two points.
> 
> **Parameters**:
> - `start`: The start position of the line cast.
> - `end`: The end position of the line cast.
> - `collideWith`: The collision layer to check against. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> 
> **Returns**: A LineCastHitResult object.
<pre class="language-typescript"><code class="lang-typescript">function LineCastWithMask(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, mask: int) -> <a data-footnote-ref href="#user-content-fn-2">LineCastHitResult</a></code></pre>
> Performs a line cast between two points, specify what to detect with a physics layer mask, returns a LineCastHitResult object
> 
<pre class="language-typescript"><code class="lang-typescript">function LineCastAll(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-2">LineCastHitResult</a>></code></pre>
> Performs a line cast between two points and returns a LineCastHitResult object for each element hit.
> 
> **Parameters**:
> - `start`: The start position of the line cast.
> - `end`: The end position of the line cast.
> - `collideWith`: The collision layer to check against. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> 
> **Returns**: A list of LineCastHitResult objects.
<pre class="language-typescript"><code class="lang-typescript">function SphereCast(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, radius: float, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Performs a sphere cast between two points.
> 
> **Parameters**:
> - `start`: The start position of the sphere cast.
> - `end`: The end position of the sphere cast.
> - `radius`: The radius of the sphere.
> - `collideWith`: The collision layer to check against. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> 
> **Returns**: The object hit (Human, Titan, etc...), or null if nothing was hit.
<pre class="language-typescript"><code class="lang-typescript">function SphereCastWithMask(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, radius: float, mask: int) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Performs a sphere cast between two points, specify what to detect with a physics layer mask, returns the object hit (Human, Titan, etc...).
> 
<pre class="language-typescript"><code class="lang-typescript">function SphereCastAll(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, radius: float, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-2">LineCastHitResult</a>></code></pre>
> Performs a sphere cast between two points and returns a LineCastHitResult object for each element hit.
> 
> **Parameters**:
> - `start`: The start position of the sphere cast.
> - `end`: The end position of the sphere cast.
> - `radius`: The radius of the sphere.
> - `collideWith`: The collision layer to check against. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> 
> **Returns**: A list of LineCastHitResult objects.
<pre class="language-typescript"><code class="lang-typescript">function BoxCast(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, dimensions: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, orientation: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Performs a box cast between two points.
> 
> **Parameters**:
> - `start`: The start position of the box cast.
> - `end`: The end position of the box cast.
> - `dimensions`: The dimensions of the box.
> - `orientation`: The orientation of the box.
> - `collideWith`: The collision layer to check against. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> 
> **Returns**: The object hit (Human, Titan, etc...), or null if nothing was hit.
<pre class="language-typescript"><code class="lang-typescript">function BoxCastAll(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, dimensions: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, orientation: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-2">LineCastHitResult</a>></code></pre>
> Performs a box cast between two points and returns a LineCastHitResult object for each element hit.
> 
> **Parameters**:
> - `start`: The start position of the box cast.
> - `end`: The end position of the box cast.
> - `dimensions`: The dimensions of the box.
> - `orientation`: The orientation of the box.
> - `collideWith`: The collision layer to check against. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> 
> **Returns**: A list of LineCastHitResult objects.
<pre class="language-typescript"><code class="lang-typescript">function ClosestPoint(point: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, collider: <a data-footnote-ref href="#user-content-fn-12">Collider</a>, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotation: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Returns a point on the given collider that is closest to the specified location.
> 
> **Parameters**:
> - `point`: The point to find the closest point to.
> - `collider`: The collider to check.
> - `position`: The position of the collider.
> - `rotation`: The rotation of the collider.
> 
> **Returns**: The closest point on the collider.
<pre class="language-typescript"><code class="lang-typescript">function ComputePenetration(colliderA: <a data-footnote-ref href="#user-content-fn-12">Collider</a>, positionA: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationA: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, colliderB: <a data-footnote-ref href="#user-content-fn-12">Collider</a>, positionB: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationB: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>) -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Compute the minimal translation required to separate the given colliders apart at specified poses.
> 
> **Parameters**:
> - `colliderA`: The first collider.
> - `positionA`: The position of the first collider.
> - `rotationA`: The rotation of the first collider.
> - `colliderB`: The second collider.
> - `positionB`: The position of the second collider.
> - `rotationB`: The rotation of the second collider.
> 
> **Returns**: Vector3.Zero if the colliders are not intersecting, otherwise the minimal translation vector.
<pre class="language-typescript"><code class="lang-typescript">function AreCollidersOverlapping(colliderA: <a data-footnote-ref href="#user-content-fn-12">Collider</a>, positionA: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationA: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, colliderB: <a data-footnote-ref href="#user-content-fn-12">Collider</a>, positionB: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, rotationB: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>) -> bool</code></pre>
> Check if the the given colliders at specified poses are apart or overlapping.
> 
> **Parameters**:
> - `colliderA`: The first collider.
> - `positionA`: The position of the first collider.
> - `rotationA`: The rotation of the first collider.
> - `colliderB`: The second collider.
> - `positionB`: The position of the second collider.
> - `rotationB`: The rotation of the second collider.
> 
> **Returns**: True if the colliders are overlapping, false otherwise.

[^0]: [Color](../Collections/Color.md)
[^1]: [Dict](../Collections/Dict.md)
[^2]: [LineCastHitResult](../Collections/LineCastHitResult.md)
[^3]: [List](../Collections/List.md)
[^4]: [Quaternion](../Collections/Quaternion.md)
[^5]: [Range](../Collections/Range.md)
[^6]: [Set](../Collections/Set.md)
[^7]: [Vector2](../Collections/Vector2.md)
[^8]: [Vector3](../Collections/Vector3.md)
[^9]: [Animation](../Component/Animation.md)
[^10]: [Animator](../Component/Animator.md)
[^11]: [AudioSource](../Component/AudioSource.md)
[^12]: [Collider](../Component/Collider.md)
[^13]: [Collision](../Component/Collision.md)
[^14]: [LightBuiltin](../Component/LightBuiltin.md)
[^15]: [LineRenderer](../Component/LineRenderer.md)
[^16]: [LodBuiltin](../Component/LodBuiltin.md)
[^17]: [MapTargetable](../Component/MapTargetable.md)
[^18]: [NavmeshObstacleBuiltin](../Component/NavmeshObstacleBuiltin.md)
[^19]: [PhysicsMaterialBuiltin](../Component/PhysicsMaterialBuiltin.md)
[^20]: [RigidbodyBuiltin](../Component/RigidbodyBuiltin.md)
[^21]: [VideoPlayer](../Component/VideoPlayer.md)
[^22]: [Character](../Entities/Character.md)
[^23]: [Horse](../Entities/Horse.md)
[^24]: [Human](../Entities/Human.md)
[^25]: [MapObject](../Entities/MapObject.md)
[^26]: [NetworkView](../Entities/NetworkView.md)
[^27]: [Player](../Entities/Player.md)
[^28]: [Prefab](../Entities/Prefab.md)
[^29]: [Shifter](../Entities/Shifter.md)
[^30]: [Titan](../Entities/Titan.md)
[^31]: [Transform](../Entities/Transform.md)
[^32]: [WallColossal](../Entities/WallColossal.md)
[^33]: [AlignEnum](../Enums/AlignEnum.md)
[^34]: [AngleUnitEnum](../Enums/AngleUnitEnum.md)
[^35]: [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md)
[^36]: [AspectRatioEnum](../Enums/AspectRatioEnum.md)
[^37]: [CameraModeEnum](../Enums/CameraModeEnum.md)
[^38]: [CharacterTypeEnum](../Enums/CharacterTypeEnum.md)
[^39]: [CollideModeEnum](../Enums/CollideModeEnum.md)
[^40]: [CollideWithEnum](../Enums/CollideWithEnum.md)
[^41]: [CollisionDetectionModeEnum](../Enums/CollisionDetectionModeEnum.md)
[^42]: [DummyAnimationEnum](../Enums/DummyAnimationEnum.md)
[^43]: [EffectNameEnum](../Enums/EffectNameEnum.md)
[^44]: [ErenAnimationEnum](../Enums/ErenAnimationEnum.md)
[^45]: [FlexDirectionEnum](../Enums/FlexDirectionEnum.md)
[^46]: [FontScaleModeEnum](../Enums/FontScaleModeEnum.md)
[^47]: [FontStyleEnum](../Enums/FontStyleEnum.md)
[^48]: [ForceModeEnum](../Enums/ForceModeEnum.md)
[^49]: [GradientModeEnum](../Enums/GradientModeEnum.md)
[^50]: [HandStateEnum](../Enums/HandStateEnum.md)
[^51]: [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
[^52]: [HumanAnimationEnum](../Enums/HumanAnimationEnum.md)
[^53]: [HumanParticleEffectEnum](../Enums/HumanParticleEffectEnum.md)
[^54]: [HumanSoundEnum](../Enums/HumanSoundEnum.md)
[^55]: [HumanStateEnum](../Enums/HumanStateEnum.md)
[^56]: [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md)
[^57]: [InputCategoryEnum](../Enums/InputCategoryEnum.md)
[^58]: [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
[^59]: [InputGeneralEnum](../Enums/InputGeneralEnum.md)
[^60]: [InputHumanEnum](../Enums/InputHumanEnum.md)
[^61]: [InputInteractionEnum](../Enums/InputInteractionEnum.md)
[^62]: [InputTitanEnum](../Enums/InputTitanEnum.md)
[^63]: [JustifyEnum](../Enums/JustifyEnum.md)
[^64]: [LanguageEnum](../Enums/LanguageEnum.md)
[^65]: [LineAlignmentEnum](../Enums/LineAlignmentEnum.md)
[^66]: [LineTextureModeEnum](../Enums/LineTextureModeEnum.md)
[^67]: [LoadoutEnum](../Enums/LoadoutEnum.md)
[^68]: [OutlineModeEnum](../Enums/OutlineModeEnum.md)
[^69]: [OverflowEnum](../Enums/OverflowEnum.md)
[^70]: [PhysicMaterialCombineEnum](../Enums/PhysicMaterialCombineEnum.md)
[^71]: [PlayerStatusEnum](../Enums/PlayerStatusEnum.md)
[^72]: [ProfileIconEnum](../Enums/ProfileIconEnum.md)
[^73]: [ProjectileNameEnum](../Enums/ProjectileNameEnum.md)
[^74]: [ScaleModeEnum](../Enums/ScaleModeEnum.md)
[^75]: [ScrollElasticityEnum](../Enums/ScrollElasticityEnum.md)
[^76]: [ShadowCastingModeEnum](../Enums/ShadowCastingModeEnum.md)
[^77]: [ShifterSoundEnum](../Enums/ShifterSoundEnum.md)
[^78]: [ShifterTypeEnum](../Enums/ShifterTypeEnum.md)
[^79]: [SliderDirectionEnum](../Enums/SliderDirectionEnum.md)
[^80]: [SpecialEnum](../Enums/SpecialEnum.md)
[^81]: [SteamStateEnum](../Enums/SteamStateEnum.md)
[^82]: [StunStateEnum](../Enums/StunStateEnum.md)
[^83]: [TSKillSoundEnum](../Enums/TSKillSoundEnum.md)
[^84]: [TeamEnum](../Enums/TeamEnum.md)
[^85]: [TextAlignEnum](../Enums/TextAlignEnum.md)
[^86]: [TextOverflowEnum](../Enums/TextOverflowEnum.md)
[^87]: [TitanAnimationEnum](../Enums/TitanAnimationEnum.md)
[^88]: [TitanDeathTypeEnum](../Enums/TitanDeathTypeEnum.md)
[^89]: [TitanSoundEnum](../Enums/TitanSoundEnum.md)
[^90]: [TitanTypeEnum](../Enums/TitanTypeEnum.md)
[^91]: [UILabelEnum](../Enums/UILabelEnum.md)
[^92]: [UnityComponentEnum](../Enums/UnityComponentEnum.md)
[^93]: [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md)
[^94]: [WeaponEnum](../Enums/WeaponEnum.md)
[^95]: [WrapEnum](../Enums/WrapEnum.md)
[^96]: [Camera](../Game/Camera.md)
[^97]: [Commands](../Game/Commands.md)
[^98]: [Cutscene](../Game/Cutscene.md)
[^99]: [ExperienceScore](../Game/ExperienceScore.md)
[^100]: [Game](../Game/Game.md)
[^101]: [Input](../Game/Input.md)
[^102]: [Locale](../Game/Locale.md)
[^103]: [Map](../Game/Map.md)
[^104]: [Network](../Game/Network.md)
[^105]: [PersistentData](../Game/PersistentData.md)
[^106]: [Physics](../Game/Physics.md)
[^107]: [RoomData](../Game/RoomData.md)
[^108]: [Service](../Game/Service.md)
[^109]: [Time](../Game/Time.md)
[^110]: [Button](../UIElements/Button.md)
[^111]: [Dropdown](../UIElements/Dropdown.md)
[^112]: [Icon](../UIElements/Icon.md)
[^113]: [Image](../UIElements/Image.md)
[^114]: [Label](../UIElements/Label.md)
[^115]: [ProgressBar](../UIElements/ProgressBar.md)
[^116]: [ScrollView](../UIElements/ScrollView.md)
[^117]: [Slider](../UIElements/Slider.md)
[^118]: [TextField](../UIElements/TextField.md)
[^119]: [Toggle](../UIElements/Toggle.md)
[^120]: [UI](../UIElements/UI.md)
[^121]: [VisualElement](../UIElements/VisualElement.md)
[^122]: [Convert](../Utility/Convert.md)
[^123]: [Json](../Utility/Json.md)
[^124]: [Math](../Utility/Math.md)
[^125]: [Random](../Utility/Random.md)
[^126]: [String](../Utility/String.md)
[^127]: [Object](../objects/Object.md)
[^128]: [Component](../objects/Component.md)
