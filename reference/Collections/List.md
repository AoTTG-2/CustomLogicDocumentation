# List
Inherits from [Object](../objects/Object.md)

Ordered collection of objects.

### Example
```csharp
values = List(1,2,1,4,115);

# Common generic list operations Map, Filter, Reduce, and Sort are supported.
# These methods take in a defined method with an expected signature and return type.

# Filter list to only unique values using set conversion.
uniques = values.ToSet().ToList();

# Accumulate values in list using reduce.
sum = values.Reduce(self.Sum2, 0);  # returns 123

# Filter list using predicate method.
filteredList = values.Filter(self.Filter);  # returns List(115)

# Transform list using mapping method.
newList = values.Map(self.TransformData);   # returns List(2,4,2,8,230)

function Sum2(a, b)
{
    return a + b;
}

function Filter(a)
{
    return a > 20;
}

function TransformData(a)
{
    return a * 2;
}
```
### Initialization
```csharp
List() // Creates an empty list.
List(parameterValues: Object) // Creates a list with the specified values.
```

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Count|int|True|The number of elements in the list.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Clear()</code></pre>
> Clear all list elements.
> 
<pre class="language-typescript"><code class="lang-typescript">function Get(index: int) -> <a data-footnote-ref href="#user-content-fn-122">Object</a><T></code></pre>
> Get the element at the specified index.
> 
> **Parameters**:
> - `index`: The index of the element to get (negative indices count from the end).
> 
<pre class="language-typescript"><code class="lang-typescript">function Set(index: int, value: <a data-footnote-ref href="#user-content-fn-122">Object</a>)</code></pre>
> Set the element at the specified index.
> 
> **Parameters**:
> - `index`: The index of the element to set (negative indices count from the end).
> - `value`: The value to set.
> 
<pre class="language-typescript"><code class="lang-typescript">function Add(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>)</code></pre>
> Add an element to the end of the list.
> 
> **Parameters**:
> - `value`: The element to add.
> 
<pre class="language-typescript"><code class="lang-typescript">function InsertAt(index: int, value: <a data-footnote-ref href="#user-content-fn-122">Object</a>)</code></pre>
> Insert an element at the specified index.
> 
> **Parameters**:
> - `index`: The index at which to insert (negative indices count from the end).
> - `value`: The element to insert.
> 
<pre class="language-typescript"><code class="lang-typescript">function RemoveAt(index: int)</code></pre>
> Remove the element at the specified index.
> 
> **Parameters**:
> - `index`: The index of the element to remove (negative indices count from the end).
> 
<pre class="language-typescript"><code class="lang-typescript">function Remove(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>)</code></pre>
> Remove the first occurrence of the specified element.
> 
> **Parameters**:
> - `value`: The element to remove.
> 
<pre class="language-typescript"><code class="lang-typescript">function Contains(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Check if the list contains the specified element.
> 
> **Parameters**:
> - `value`: The element to check for.
> 
<pre class="language-typescript"><code class="lang-typescript">function Sort()</code></pre>
> Sort the list.
> 
<pre class="language-typescript"><code class="lang-typescript">function SortCustom(method: function)</code></pre>
> Sort the list using a custom method, expects a method with the signature int method(a,b).
> 
> **Parameters**:
> - `method`: The comparison method that returns an int: negative if a < b, 0 if a == b, positive if a > b.
> 
<pre class="language-typescript"><code class="lang-typescript">function Filter(method: function) -> <a data-footnote-ref href="#user-content-fn-3">List</a><T></code></pre>
> Filter the list using a custom method, expects a method with the signature bool method(element).
> 
> **Parameters**:
> - `method`: The predicate method that returns true for elements to keep.
> 
<pre class="language-typescript"><code class="lang-typescript">function Map(method: function) -> <a data-footnote-ref href="#user-content-fn-3">List</a><T></code></pre>
> Map the list using a custom method, expects a method with the signature object method(element).
> 
> **Parameters**:
> - `method`: The transformation method that returns the mapped value for each element.
> 
<pre class="language-typescript"><code class="lang-typescript">function Reduce(method: function, initialValue: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> <a data-footnote-ref href="#user-content-fn-122">Object</a></code></pre>
> Reduce the list using a custom method, expects a method with the signature object method(acc, element).
> 
> **Parameters**:
> - `method`: The accumulation method that combines the accumulator with each element.
> - `initialValue`: The initial accumulator value.
> 
<pre class="language-typescript"><code class="lang-typescript">function Randomize() -> <a data-footnote-ref href="#user-content-fn-3">List</a><T></code></pre>
> Returns a randomized version of the list.
> 
<pre class="language-typescript"><code class="lang-typescript">function ToSet() -> <a data-footnote-ref href="#user-content-fn-6">Set</a><T></code></pre>
> Convert the list to a set.
> 
<pre class="language-typescript"><code class="lang-typescript">function Copy() -> <a data-footnote-ref href="#user-content-fn-3">List</a><T></code></pre>
> Copy the list to a new list.
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
[^95]: [Cutscene](../Game/Cutscene.md)
[^96]: [Game](../Game/Game.md)
[^97]: [Input](../Game/Input.md)
[^98]: [Locale](../Game/Locale.md)
[^99]: [Map](../Game/Map.md)
[^100]: [Network](../Game/Network.md)
[^101]: [PersistentData](../Game/PersistentData.md)
[^102]: [Physics](../Game/Physics.md)
[^103]: [RoomData](../Game/RoomData.md)
[^104]: [Time](../Game/Time.md)
[^105]: [Button](../UIElements/Button.md)
[^106]: [Dropdown](../UIElements/Dropdown.md)
[^107]: [Icon](../UIElements/Icon.md)
[^108]: [Image](../UIElements/Image.md)
[^109]: [Label](../UIElements/Label.md)
[^110]: [ProgressBar](../UIElements/ProgressBar.md)
[^111]: [ScrollView](../UIElements/ScrollView.md)
[^112]: [Slider](../UIElements/Slider.md)
[^113]: [TextField](../UIElements/TextField.md)
[^114]: [Toggle](../UIElements/Toggle.md)
[^115]: [UI](../UIElements/UI.md)
[^116]: [VisualElement](../UIElements/VisualElement.md)
[^117]: [Convert](../Utility/Convert.md)
[^118]: [Json](../Utility/Json.md)
[^119]: [Math](../Utility/Math.md)
[^120]: [Random](../Utility/Random.md)
[^121]: [String](../Utility/String.md)
[^122]: [Object](../objects/Object.md)
[^123]: [Component](../objects/Component.md)
