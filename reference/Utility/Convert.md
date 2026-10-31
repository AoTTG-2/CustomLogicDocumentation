# Convert
Inherits from [Object](../objects/Object.md)

Converting objects to different types.

### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function ToFloat(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> float</code></pre>
> Converts a value to a float.
> 
> **Parameters**:
> - `value`: The value to convert (can be string, float, int, or bool).
> 
> **Returns**: The converted float value.
<pre class="language-typescript"><code class="lang-typescript">function ToInt(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> int</code></pre>
> Converts a value to an int.
> 
> **Parameters**:
> - `value`: The value to convert (can be string, float, int, or bool).
> 
> **Returns**: The converted int value.
<pre class="language-typescript"><code class="lang-typescript">function ToBool(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> bool</code></pre>
> Converts a value to a bool.
> 
> **Parameters**:
> - `value`: The value to convert (can be string, float, int, or bool).
> 
> **Returns**: The converted bool value.
<pre class="language-typescript"><code class="lang-typescript">function ToString(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> string</code></pre>
> Converts a value to a string.
> 
> **Parameters**:
> - `value`: The value to convert.
> 
> **Returns**: The converted string value.
<pre class="language-typescript"><code class="lang-typescript">function IsFloat(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> bool</code></pre>
> Checks if the value is a float.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is a float, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsInt(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> bool</code></pre>
> Checks if the value is an int.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is an int, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsBool(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> bool</code></pre>
> Checks if the value is a bool.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is a bool, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsString(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> bool</code></pre>
> Checks if the value is a string.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is a string, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsObject(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> bool</code></pre>
> Checks if the value is an object.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is an object, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsList(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> bool</code></pre>
> Checks if the value is a list.
> 
> **Parameters**:
> - `value`: The value to check.
> 
> **Returns**: True if the value is a list, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function IsDict(value: <a data-footnote-ref href="#user-content-fn-127">Object</a>) -> bool</code></pre>
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
<pre class="language-typescript"><code class="lang-typescript">function DefineVariable(cInstance: class, variableName: string, value: <a data-footnote-ref href="#user-content-fn-127">Object</a>)</code></pre>
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
