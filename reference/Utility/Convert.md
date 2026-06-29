# Convert
Inherits from [Object](../objects/Object.md)

Converting objects to different types.

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function ToFloat(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> float</code></pre>
> Converts a value to a float.
> 
> **Parameters**:
> - `value`: The value to convert (can be string, float, int, or bool).
> 
> **Returns**: The converted float value.
<pre class="language-typescript"><code class="lang-typescript">function ToInt(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> int</code></pre>
> Converts a value to an int.
> 
> **Parameters**:
> - `value`: The value to convert (can be string, float, int, or bool).
> 
> **Returns**: The converted int value.
<pre class="language-typescript"><code class="lang-typescript">function ToBool(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Converts a value to a bool.
> 
> **Parameters**:
> - `value`: The value to convert (can be string, float, int, or bool).
> 
> **Returns**: The converted bool value.
<pre class="language-typescript"><code class="lang-typescript">function ToString(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> string</code></pre>
> Converts a value to a string.
> 
> **Parameters**:
> - `value`: The value to convert.
> 
> **Returns**: The converted string value.
<pre class="language-typescript"><code class="lang-typescript">function IsFloat(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Checks if the value is a float.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is a float, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsInt(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Checks if the value is an int.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is an int, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsBool(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Checks if the value is a bool.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is a bool, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsString(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Checks if the value is a string.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is a string, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsObject(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Checks if the value is an object.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is an object, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsList(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Checks if the value is a list.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is a list, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsDict(value: <a data-footnote-ref href="#user-content-fn-122">Object</a>) -> bool</code></pre>
> Checks if the value is a dictionary.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is a dictionary, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function HasVariable(cInstance: class, variableName: string) -> bool</code></pre>
> Checks if the class instance has a variable.
> 
> **Parameters**:
> - `cInstance`: The class instance to check.
> - `variableName`: The name of the variable to check for.
> 
> **Returns**: True if the class instance has the variable, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function DefineVariable(cInstance: class, variableName: string, value: <a data-footnote-ref href="#user-content-fn-122">Object</a>)</code></pre>
> Defines a variable for the class instance.
> 
> **Parameters**:
> - `cInstance`: The class instance to define the variable on.
> - `variableName`: The name of the variable to define.
> - `value`: The value to assign to the variable.
> 
<pre class="language-typescript"><code class="lang-typescript">function RemoveVariable(cInstance: class, variableName: string)</code></pre>
> Removes a variable from the class instance.
> 
> **Parameters**:
> - `cInstance`: The class instance to remove the variable from.
> - `variableName`: The name of the variable to remove.
> 
<pre class="language-typescript"><code class="lang-typescript">function HasMethod(cInstance: class, methodName: string) -> bool</code></pre>
> Checks if the class instance has a method.
> 
> **Parameters**:
> - `cInstance`: The class instance to check.
> - `methodName`: The name of the method to check for.
> 
> **Returns**: True if the class instance has the method, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function GetType(cInstance: class) -> string</code></pre>
> Gets the type of the class instance.
> 
> **Parameters**:
> - `cInstance`: The class instance to get the type of.
> 
> **Returns**: The class name of the instance.

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
