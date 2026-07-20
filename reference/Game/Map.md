# Map
Inherits from [Object](../objects/Object.md)

Finding, creating, and destroying map objects.

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function FindAllMapObjects() -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-24">MapObject</a>></code></pre>
> Find all map objects.
> 
> **Returns**: A list of all map objects.
<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectByName(objectName: string) -> <a data-footnote-ref href="#user-content-fn-24">MapObject</a></code></pre>
> Find a map object by name.
> 
> **Parameters**:
> - `objectName`: The name of the map object to find.
> 
> **Returns**: The map object if found, null otherwise.
<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectsByName(objectName: string) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-24">MapObject</a>></code></pre>
> Find all map objects by name.
> 
> **Parameters**:
> - `objectName`: The name of the map objects to find.
> 
> **Returns**: A list of map objects with the specified name.
<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectsByRegex(pattern: string, sorted: bool = False) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-24">MapObject</a>></code></pre>
> Find all map objects by regex pattern.
> 
> **Parameters**:
> - `pattern`: The regex pattern to match against map object names.
> - `sorted`: If true, sorts the results by name (default: false).
> 
> **Returns**: A list of map objects matching the regex pattern.
<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectByComponent(className: string) -> <a data-footnote-ref href="#user-content-fn-24">MapObject</a></code></pre>
> Find all map objects by component.
> 
> **Parameters**:
> - `className`: The class name of the component to search for.
> 
> **Returns**: The first map object with the specified component, or null if not found.
<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectsByComponent(className: string) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-24">MapObject</a>></code></pre>
> Find all map objects by component.
> 
> **Parameters**:
> - `className`: The class name of the component to search for.
> 
> **Returns**: A list of map objects with the specified component.
<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectByID(id: int) -> <a data-footnote-ref href="#user-content-fn-24">MapObject</a></code></pre>
> Find a map object by ID.
> 
> **Parameters**:
> - `id`: The ID of the map object to find.
> 
> **Returns**: The map object if found, null otherwise.
<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectByTag(tag: string) -> <a data-footnote-ref href="#user-content-fn-24">MapObject</a></code></pre>
> Find a map object by tag.
> 
> **Parameters**:
> - `tag`: The tag to search for.
> 
> **Returns**: The first map object with the specified tag, or null if not found.
<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectsByTag(tag: string) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-24">MapObject</a>></code></pre>
> Find all map objects by tag.
> 
> **Parameters**:
> - `tag`: The tag to search for.
> 
> **Returns**: A list of map objects with the specified tag.
<pre class="language-typescript"><code class="lang-typescript">function FindMapObjectsByPlayer(player: <a data-footnote-ref href="#user-content-fn-26">Player</a>) -> <a data-footnote-ref href="#user-content-fn-3">List</a><<a data-footnote-ref href="#user-content-fn-24">MapObject</a>></code></pre>
> Find a map objects of Player.
> 
> **Parameters**:
> - `player`: The player to find map objects for.
> 
> **Returns**: A list of map objects owned by the player.
<pre class="language-typescript"><code class="lang-typescript">function CreateMapObject(prefab: <a data-footnote-ref href="#user-content-fn-27">Prefab</a>, position: <a data-footnote-ref href="#user-content-fn-8">Vector3</a> = null, rotation: <a data-footnote-ref href="#user-content-fn-8">Vector3</a> = null, scale: <a data-footnote-ref href="#user-content-fn-8">Vector3</a> = null) -> <a data-footnote-ref href="#user-content-fn-24">MapObject</a></code></pre>
> Create a new map object.
> 
> **Parameters**:
> - `prefab`: The prefab to instantiate.
> - `position`: The position to spawn at (default: null, uses prefab position).
> - `rotation`: The rotation to spawn with (default: null, uses prefab rotation).
> - `scale`: The scale to spawn with (default: null, uses prefab scale).
> 
> **Returns**: The created map object.
<pre class="language-typescript"><code class="lang-typescript">function CreateMapObjectRaw(prefab: string) -> <a data-footnote-ref href="#user-content-fn-24">MapObject</a></code></pre>
> Create a new map object.
> 
> **Parameters**:
> - `prefab`: The serialized prefab string to instantiate.
> 
> **Returns**: The created map object.
<pre class="language-typescript"><code class="lang-typescript">function PrefabFromMapObject(mapObject: <a data-footnote-ref href="#user-content-fn-24">MapObject</a>, clearComponents: bool = False) -> <a data-footnote-ref href="#user-content-fn-27">Prefab</a></code></pre>
> Create a new prefab object from the current object.
> 
> **Parameters**:
> - `mapObject`: The map object to create a prefab from.
> - `clearComponents`: If true, clears all components from the prefab (default: false).
> 
> **Returns**: The created prefab.
<pre class="language-typescript"><code class="lang-typescript">function DestroyMapObject(mapObject: <a data-footnote-ref href="#user-content-fn-24">MapObject</a>, includeChildren: bool)</code></pre>
> Destroy a map object.
> 
> **Parameters**:
> - `mapObject`: The map object to destroy.
> - `includeChildren`: If true, also destroys all child objects.
> 
<pre class="language-typescript"><code class="lang-typescript">function CopyMapObject(mapObject: <a data-footnote-ref href="#user-content-fn-24">MapObject</a>, includeChildren: bool = True) -> <a data-footnote-ref href="#user-content-fn-24">MapObject</a></code></pre>
> Copy a map object.
> 
> **Parameters**:
> - `mapObject`: The map object to copy.
> - `includeChildren`: If true, also copies all child objects (default: true).
> 
> **Returns**: The copied map object.
<pre class="language-typescript"><code class="lang-typescript">function DestroyMapTargetable(targetable: <a data-footnote-ref href="#user-content-fn-17">MapTargetable</a>)</code></pre>
> Destroy a map targetable.
> 
> **Parameters**:
> - `targetable`: The map targetable to destroy.
> 
<pre class="language-typescript"><code class="lang-typescript">function UpdateNavMesh()</code></pre>
> Update the nav mesh.
> 
<pre class="language-typescript"><code class="lang-typescript">function UpdateNavMeshAsync()</code></pre>
> Update the nav mesh asynchronously.
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
