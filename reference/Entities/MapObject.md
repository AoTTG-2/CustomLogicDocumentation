# MapObject
Inherits from [Object](../objects/Object.md)

MapObject represents a map object created in the editor or spawned at runtime using Map static methods.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Static|bool|True|Object does not move.|
|Position|[Vector3](../Collections/Vector3.md)|False|The position of the object.|
|LocalPosition|[Vector3](../Collections/Vector3.md)|False|The local position of the object.|
|Rotation|[Vector3](../Collections/Vector3.md)|False|The rotation of the object.|
|LocalRotation|[Vector3](../Collections/Vector3.md)|False|The local rotation of the object.|
|QuaternionRotation|[Quaternion](../Collections/Quaternion.md)|False|The rotation of the object as a quaternion.|
|QuaternionLocalRotation|[Quaternion](../Collections/Quaternion.md)|False|The local rotation of the object as a quaternion.|
|Forward|[Vector3](../Collections/Vector3.md)|False|The forward direction of the object.|
|Up|[Vector3](../Collections/Vector3.md)|False|The up direction of the object.|
|Right|[Vector3](../Collections/Vector3.md)|False|The right direction of the object.|
|Scale|[Vector3](../Collections/Vector3.md)|False|The scale of the object.|
|Name|string|True|The name of the object.|
|Parent|[Object](../objects/Object.md)|False|The parent of the object.|
|Active|bool|False|Whether the object is active.|
|ActiveInHierarchy|bool|True||
|Transform|[Transform](../Entities/Transform.md)|True|The transform of the object.|
|HasRenderer|bool|True|Whether the object has a renderer.|
|Color|[Color](../Collections/Color.md)|False|The color of the object.|
|TextureTilingX|float|False|The x tiling of the object's texture.|
|TextureTilingY|float|False|The y tiling of the object's texture.|
|TextureOffsetX|float|False|The x offset of the object's texture.|
|TextureOffsetY|float|False|The y offset of the object's texture.|
|ID|int|True|The ID of the object.|
|Tag|string|False|The tag of the object.|
|Layer|int|False|The layer of the object.|
|Rigidbody|[RigidbodyBuiltin](../Component/RigidbodyBuiltin.md)|True|The Rigidbody component of the MapObject, is null if not added.|
|NetworkView|[NetworkView](../Entities/NetworkView.md)|False|The NetworkView attached to the MapObject, is null if not initialized yet.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function AddComponent(name: string) -> component</code></pre>
> Add a component to the object.
> 
> **Parameters**:
> - `name`: The name of the component to add.
> 
> **Returns**: The added component instance.
<pre class="language-typescript"><code class="lang-typescript">function RemoveComponent(name: string)</code></pre>
> Remove a component from the object.
> 
> **Parameters**:
> - `name`: The name of the component to remove.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetComponent(name: string) -> component</code></pre>
> Get a component from the object.
> 
> **Parameters**:
> - `name`: The name of the component to get.
> 
> **Returns**: The component instance, or null if not found.
<pre class="language-typescript"><code class="lang-typescript">function GetUnityComponent(name: string) -> BuiltinComponentInstance</code></pre>
> Get a custom logic unity component from the object.
> 
> **Parameters**:
> - `name`: The UnityComponentEnum to get.
> 
> **Returns**: The component instance, or null if not found.
<pre class="language-typescript"><code class="lang-typescript">function SetComponentEnabled(name: string, enabled: bool)</code></pre>
> Set whether a component is enabled.
> 
> **Parameters**:
> - `name`: The name of the component.
> - `enabled`: Whether the component should be enabled.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetComponentsEnabled(enabled: bool)</code></pre>
> Set whether all components are enabled.
> 
> **Parameters**:
> - `enabled`: Whether all components should be enabled.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddSphereCollider(collideMode: string, collideWith: string, center: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, radius: float)</code></pre>
> Add a sphere collider to the object.
> 
> **Parameters**:
> - `collideMode`: The collision mode. Refer to [CollideModeEnum](../Enums/CollideModeEnum.md)
> - `collideWith`: What the collider should collide with. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> - `center`: The center position of the sphere collider.
> - `radius`: The radius of the sphere collider.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddBoxCollider(collideMode: string, collideWith: string, center: <a data-footnote-ref href="#user-content-fn-8">Vector3</a> = null, size: <a data-footnote-ref href="#user-content-fn-8">Vector3</a> = null)</code></pre>
> Add a box collider to the object.
> 
> **Parameters**:
> - `collideMode`: The collision mode. Refer to [CollideModeEnum](../Enums/CollideModeEnum.md)
> - `collideWith`: What the collider should collide with. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> - `center`: The center position of the box collider (optional, defaults to calculated bounds).
> - `size`: The size of the box collider (optional, defaults to calculated bounds).
> 
<pre class="language-typescript"><code class="lang-typescript">function SetCollideWith(collideWith: string)</code></pre>
> Set the collideWith property for all colliders on this object and its children.
This changes which layers the colliders can collide with.
> 
> **Parameters**:
> - `collideWith`: What the colliders should collide with. Refer to [CollideWithEnum](../Enums/CollideWithEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function SetCollideMode(collideMode: string)</code></pre>
> Set the collideMode property for all colliders on this object and its children.
This changes whether the colliders are physical, region triggers, or disabled.
> 
> **Parameters**:
> - `collideMode`: The collision mode to apply to all colliders. Refer to [CollideModeEnum](../Enums/CollideModeEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function AddSphereTarget(team: string, center: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, radius: float) -> <a data-footnote-ref href="#user-content-fn-17">MapTargetable</a></code></pre>
> Add a sphere target to the object.
> 
> **Parameters**:
> - `team`: The team that can target this. Refer to [TeamEnum](../Enums/TeamEnum.md)
> - `center`: The center position of the sphere target.
> - `radius`: The radius of the sphere target.
> 
> **Returns**: The created targetable object.
<pre class="language-typescript"><code class="lang-typescript">function AddBoxTarget(team: string, center: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>, size: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-17">MapTargetable</a></code></pre>
> Add a box target to the object.
> 
> **Parameters**:
> - `team`: The team that can target this. Refer to [TeamEnum](../Enums/TeamEnum.md)
> - `center`: The center position of the box target.
> - `size`: The size of the box target.
> 
> **Returns**: The created targetable object.
<pre class="language-typescript"><code class="lang-typescript">function GetChild(name: string) -> <a data-footnote-ref href="#user-content-fn-25">MapObject</a></code></pre>
> Get a child object by name.
> 
> **Parameters**:
> - `name`: The name of the child object to get.
> 
> **Returns**: The child object if found, null otherwise.
<pre class="language-typescript"><code class="lang-typescript">function GetChildren() -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-25">MapObject</a>></code></pre>
> Get all child objects.
> 
> **Returns**: A list of all child objects.
<pre class="language-typescript"><code class="lang-typescript">function GetTransform(name: string) -> <a data-footnote-ref href="#user-content-fn-31">Transform</a></code></pre>
> Get a child transform by name.
> 
> **Parameters**:
> - `name`: The name of the transform to get.
> 
> **Returns**: The transform if found, null otherwise.
<pre class="language-typescript"><code class="lang-typescript">function SetColorAll(color: <a data-footnote-ref href="#user-content-fn-0">Color</a>)</code></pre>
> Set the color of all renderers on the object.
> 
> **Parameters**:
> - `color`: The color to set.
> 
<pre class="language-typescript"><code class="lang-typescript">function InBounds(position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a>) -> bool</code></pre>
> Check if a position is within the object's bounds.
> 
> **Parameters**:
> - `position`: The position to check.
> 
> **Returns**: True if the position is within the bounds, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function GetBoundsAverageCenter() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Get the bounds average center.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetBoundsCenter() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Get the bounds center.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetBoundsSize() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Get the bounds size.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetBoundsMin() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Get the bounds min.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetBoundsMax() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Get the bounds max.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetBoundsExtents() -> <a data-footnote-ref href="#user-content-fn-8">Vector3</a></code></pre>
> Get the bounds extents.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetCorners() -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-8">Vector3</a>></code></pre>
> Get the corners of the bounds.
> 
<pre class="language-typescript"><code class="lang-typescript">function HasTag(tag: string) -> bool</code></pre>
> Whether or not the object has the given tag.
> 
> **Parameters**:
> - `tag`: The tag to check for.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddBuiltinComponent(name: string) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Add a builtin component to the MapObject.
> 
> **Parameters**:
> - `name`: The name of the builtin component to add.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddRigidbody() -> <a data-footnote-ref href="#user-content-fn-20">RigidbodyBuiltin</a></code></pre>
> Add a Rigidbody component to the MapObject.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetBuiltinComponent(name: string) -> <a data-footnote-ref href="#user-content-fn-127">Object</a></code></pre>
> Gets a builtin component to the MapObject.
> 
> **Parameters**:
> - `name`: The name of the builtin component to get.
> 
<pre class="language-typescript"><code class="lang-typescript">function RemoveBuiltinComponent(name: string)</code></pre>
> Remove a builtin component from the MapObject.
> 
> **Parameters**:
> - `name`: The name of the builtin component to remove.
> 
<pre class="language-typescript"><code class="lang-typescript">function ConvertToCSV() -> string</code></pre>
> Serialize the current object to a csv.
> 

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
