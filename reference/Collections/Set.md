# Set
Inherits from [Object](../objects/Object.md)

Collection of unique elements.

### Initialization
```csharp
Set() // Creates an empty set.
Set(parameterValues: Object) // Creates a set with the specified values.
```

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Count|int|True|The number of elements in the set.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Clear()</code></pre>
> Clear all set elements.
> 
<pre class="language-typescript"><code class="lang-typescript">function Contains(value: <a data-footnote-ref href="#user-content-fn-124">Object</a>) -> bool</code></pre>
> Check if the set contains the specified element.
> 
> **Parameters**:
> - `value`: The element to check for.
> 
<pre class="language-typescript"><code class="lang-typescript">function Add(value: <a data-footnote-ref href="#user-content-fn-124">Object</a>)</code></pre>
> Add an element to the set.
> 
> **Parameters**:
> - `value`: The element to add.
> 
<pre class="language-typescript"><code class="lang-typescript">function Remove(value: <a data-footnote-ref href="#user-content-fn-124">Object</a>)</code></pre>
> Remove the element from the set.
> 
> **Parameters**:
> - `value`: The element to remove.
> 
<pre class="language-typescript"><code class="lang-typescript">function Union(set: <a data-footnote-ref href="#user-content-fn-6">Set</a>)</code></pre>
> Union with another set (adds all elements from the other set to this set).
> 
> **Parameters**:
> - `set`: The set to union with.
> 
<pre class="language-typescript"><code class="lang-typescript">function Intersect(set: <a data-footnote-ref href="#user-content-fn-6">Set</a>)</code></pre>
> Intersect with another set (keeps only elements that are in both sets).
> 
> **Parameters**:
> - `set`: The set to intersect with.
> 
<pre class="language-typescript"><code class="lang-typescript">function Difference(set: <a data-footnote-ref href="#user-content-fn-6">Set</a>)</code></pre>
> Difference with another set (removes all elements that are in the other set).
> 
> **Parameters**:
> - `set`: The set to compute the difference with.
> 
<pre class="language-typescript"><code class="lang-typescript">function IsSubsetOf(set: <a data-footnote-ref href="#user-content-fn-6">Set</a>) -> bool</code></pre>
> Check if the set is a subset of another set.
> 
> **Parameters**:
> - `set`: The set to check against.
> 
<pre class="language-typescript"><code class="lang-typescript">function IsSupersetOf(set: <a data-footnote-ref href="#user-content-fn-6">Set</a>) -> bool</code></pre>
> Check if the set is a superset of another set.
> 
> **Parameters**:
> - `set`: The set to check against.
> 
<pre class="language-typescript"><code class="lang-typescript">function IsProperSubsetOf(set: <a data-footnote-ref href="#user-content-fn-6">Set</a>) -> bool</code></pre>
> Check if the set is a proper subset of another set (subset but not equal).
> 
> **Parameters**:
> - `set`: The set to check against.
> 
<pre class="language-typescript"><code class="lang-typescript">function IsProperSupersetOf(set: <a data-footnote-ref href="#user-content-fn-6">Set</a>) -> bool</code></pre>
> Check if the set is a proper superset of another set (superset but not equal).
> 
> **Parameters**:
> - `set`: The set to check against.
> 
<pre class="language-typescript"><code class="lang-typescript">function Overlaps(set: <a data-footnote-ref href="#user-content-fn-6">Set</a>) -> bool</code></pre>
> Check if the set overlaps with another set (has at least one element in common).
> 
> **Parameters**:
> - `set`: The set to check against.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetEquals(set: <a data-footnote-ref href="#user-content-fn-6">Set</a>) -> bool</code></pre>
> Check if the set has the same elements as another set.
> 
> **Parameters**:
> - `set`: The set to compare with.
> 
<pre class="language-typescript"><code class="lang-typescript">function ToList() -> <a data-footnote-ref href="#user-content-fn-3">List</a><T></code></pre>
> Convert the set to a list.
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
