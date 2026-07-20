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
<pre class="language-typescript"><code class="lang-typescript">function SphereCast(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, radius: float, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-124">Object</a></code></pre>
> Performs a sphere cast between two points.
> 
> **Parameters**:
> - `start`: The start position of the sphere cast.
> - `end`: The end position of the sphere cast.
> - `radius`: The radius of the sphere.
> - `collideWith`: The collision layer to check against. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> 
> **Returns**: The object hit (Human, Titan, etc...), or null if nothing was hit.
<pre class="language-typescript"><code class="lang-typescript">function SphereCastWithMask(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, radius: float, mask: int) -> <a data-footnote-ref href="#user-content-fn-124">Object</a></code></pre>
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
<pre class="language-typescript"><code class="lang-typescript">function BoxCast(start: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, end: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, dimensions: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, orientation: <a data-footnote-ref href="#user-content-fn-4">Quaternion</a>, collideWith: string) -> <a data-footnote-ref href="#user-content-fn-124">Object</a></code></pre>
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
[^23]: [Human](../Entities/Human.md)
[^24]: [MapObject](../Entities/MapObject.md)
[^25]: [NetworkView](../Entities/NetworkView.md)
[^26]: [Player](../Entities/Player.md)
[^27]: [Prefab](../Entities/Prefab.md)
[^28]: [Shifter](../Entities/Shifter.md)
[^29]: [Titan](../Entities/Titan.md)
[^30]: [Transform](../Entities/Transform.md)
[^31]: [WallColossal](../Entities/WallColossal.md)
[^32]: [AlignEnum](../Enums/AlignEnum.md)
[^33]: [AngleUnitEnum](../Enums/AngleUnitEnum.md)
[^34]: [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md)
[^35]: [AspectRatioEnum](../Enums/AspectRatioEnum.md)
[^36]: [CameraModeEnum](../Enums/CameraModeEnum.md)
[^37]: [CharacterTypeEnum](../Enums/CharacterTypeEnum.md)
[^38]: [CollideModeEnum](../Enums/CollideModeEnum.md)
[^39]: [CollideWithEnum](../Enums/CollideWithEnum.md)
[^40]: [CollisionDetectionModeEnum](../Enums/CollisionDetectionModeEnum.md)
[^41]: [DummyAnimationEnum](../Enums/DummyAnimationEnum.md)
[^42]: [EffectNameEnum](../Enums/EffectNameEnum.md)
[^43]: [ErenAnimationEnum](../Enums/ErenAnimationEnum.md)
[^44]: [FlexDirectionEnum](../Enums/FlexDirectionEnum.md)
[^45]: [FontScaleModeEnum](../Enums/FontScaleModeEnum.md)
[^46]: [FontStyleEnum](../Enums/FontStyleEnum.md)
[^47]: [ForceModeEnum](../Enums/ForceModeEnum.md)
[^48]: [GradientModeEnum](../Enums/GradientModeEnum.md)
[^49]: [HandStateEnum](../Enums/HandStateEnum.md)
[^50]: [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
[^51]: [HumanAnimationEnum](../Enums/HumanAnimationEnum.md)
[^52]: [HumanParticleEffectEnum](../Enums/HumanParticleEffectEnum.md)
[^53]: [HumanSoundEnum](../Enums/HumanSoundEnum.md)
[^54]: [HumanStateEnum](../Enums/HumanStateEnum.md)
[^55]: [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md)
[^56]: [InputCategoryEnum](../Enums/InputCategoryEnum.md)
[^57]: [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
[^58]: [InputGeneralEnum](../Enums/InputGeneralEnum.md)
[^59]: [InputHumanEnum](../Enums/InputHumanEnum.md)
[^60]: [InputInteractionEnum](../Enums/InputInteractionEnum.md)
[^61]: [InputTitanEnum](../Enums/InputTitanEnum.md)
[^62]: [JustifyEnum](../Enums/JustifyEnum.md)
[^63]: [LanguageEnum](../Enums/LanguageEnum.md)
[^64]: [LineAlignmentEnum](../Enums/LineAlignmentEnum.md)
[^65]: [LineTextureModeEnum](../Enums/LineTextureModeEnum.md)
[^66]: [LoadoutEnum](../Enums/LoadoutEnum.md)
[^67]: [OutlineModeEnum](../Enums/OutlineModeEnum.md)
[^68]: [OverflowEnum](../Enums/OverflowEnum.md)
[^69]: [PhysicMaterialCombineEnum](../Enums/PhysicMaterialCombineEnum.md)
[^70]: [PlayerStatusEnum](../Enums/PlayerStatusEnum.md)
[^71]: [ProfileIconEnum](../Enums/ProfileIconEnum.md)
[^72]: [ProjectileNameEnum](../Enums/ProjectileNameEnum.md)
[^73]: [ScaleModeEnum](../Enums/ScaleModeEnum.md)
[^74]: [ScrollElasticityEnum](../Enums/ScrollElasticityEnum.md)
[^75]: [ShadowCastingModeEnum](../Enums/ShadowCastingModeEnum.md)
[^76]: [ShifterSoundEnum](../Enums/ShifterSoundEnum.md)
[^77]: [ShifterTypeEnum](../Enums/ShifterTypeEnum.md)
[^78]: [SliderDirectionEnum](../Enums/SliderDirectionEnum.md)
[^79]: [SpecialEnum](../Enums/SpecialEnum.md)
[^80]: [SteamStateEnum](../Enums/SteamStateEnum.md)
[^81]: [StunStateEnum](../Enums/StunStateEnum.md)
[^82]: [TeamEnum](../Enums/TeamEnum.md)
[^83]: [TextAlignEnum](../Enums/TextAlignEnum.md)
[^84]: [TextOverflowEnum](../Enums/TextOverflowEnum.md)
[^85]: [TitanAnimationEnum](../Enums/TitanAnimationEnum.md)
[^86]: [TitanSoundEnum](../Enums/TitanSoundEnum.md)
[^87]: [TitanTypeEnum](../Enums/TitanTypeEnum.md)
[^88]: [TSKillSoundEnum](../Enums/TSKillSoundEnum.md)
[^89]: [UILabelEnum](../Enums/UILabelEnum.md)
[^90]: [UnityComponentEnum](../Enums/UnityComponentEnum.md)
[^91]: [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md)
[^92]: [WeaponEnum](../Enums/WeaponEnum.md)
[^93]: [WrapEnum](../Enums/WrapEnum.md)
[^94]: [Camera](../Game/Camera.md)
[^95]: [Commands](../Game/Commands.md)
[^96]: [Cutscene](../Game/Cutscene.md)
[^97]: [Game](../Game/Game.md)
[^98]: [Input](../Game/Input.md)
[^99]: [Locale](../Game/Locale.md)
[^100]: [Map](../Game/Map.md)
[^101]: [Network](../Game/Network.md)
[^102]: [PersistentData](../Game/PersistentData.md)
[^103]: [Physics](../Game/Physics.md)
[^104]: [RoomData](../Game/RoomData.md)
[^105]: [Service](../Game/Service.md)
[^106]: [Time](../Game/Time.md)
[^107]: [Button](../UIElements/Button.md)
[^108]: [Dropdown](../UIElements/Dropdown.md)
[^109]: [Icon](../UIElements/Icon.md)
[^110]: [Image](../UIElements/Image.md)
[^111]: [Label](../UIElements/Label.md)
[^112]: [ProgressBar](../UIElements/ProgressBar.md)
[^113]: [ScrollView](../UIElements/ScrollView.md)
[^114]: [Slider](../UIElements/Slider.md)
[^115]: [TextField](../UIElements/TextField.md)
[^116]: [Toggle](../UIElements/Toggle.md)
[^117]: [UI](../UIElements/UI.md)
[^118]: [VisualElement](../UIElements/VisualElement.md)
[^119]: [Convert](../Utility/Convert.md)
[^120]: [Json](../Utility/Json.md)
[^121]: [Math](../Utility/Math.md)
[^122]: [Random](../Utility/Random.md)
[^123]: [String](../Utility/String.md)
[^124]: [Object](../objects/Object.md)
[^125]: [Component](../objects/Component.md)
