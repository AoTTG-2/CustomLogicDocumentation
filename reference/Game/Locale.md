# Locale
Inherits from [Object](../objects/Object.md)

Internationalization (Locale) utility for managing localized strings.
Supports single-level (non-recursive) language fallbacks and automatic UI language detection.

### Example
```csharp
# Register individual strings for different languages
Locale.Set(LanguageEnum.English, "welcome", "Welcome to the game!");
Locale.Set(LanguageEnum.Russian, "welcome", "Добро пожаловать в игру!");
Locale.Set(LanguageEnum.Chinese, "welcome", "你好");

Game.Print("welcome: " + Locale.Get("welcome"));

# Register multiple strings at once using a dictionary
englishStrings = Dict();
englishStrings.Set("hello", "Hello");
englishStrings.Set("goodbye", "Goodbye");
englishStrings.Set("score", "Score: {0}");
Locale.RegisterLanguage(LanguageEnum.English, englishStrings);

russianStrings = Dict();
russianStrings.Set("hello", "Привет");
russianStrings.Set("goodbye", "Пока");
russianStrings.Set("score", "Счет: {0}");
Locale.RegisterLanguage(LanguageEnum.Russian, russianStrings);

chineseStrings = Dict();
chineseStrings.Set("hello", "你好");
chineseStrings.Set("goodbye", "再见");
chineseStrings.Set("score", "分数: {0}");
Locale.RegisterLanguage(LanguageEnum.Chinese, chineseStrings);

# Get localized strings (automatically uses current UI language)
Game.Print("hello: " + Locale.Get("hello"));
Game.Print("goodbye: " + Locale.Get("goodbye"));

params = List();
params.Add(83);
Game.Print("score: " + String.FormatFromList(Locale.Get("score"), params));

# Register all strings from internal JSON files for a specific category
# Use internal:// prefix to specify internal localization files
Locale.RegisterLanguages("internal://BasicTutorialMap");

Game.Print("Name.Game: " + Locale.Get("Name.Game"));
Game.Print("Name.Tutorial: " + Locale.Get("Name.Tutorial"));
Game.Print("Stage.Introduction: " + Locale.Get("Stage.Introduction"));

# Register all strings from external JSON files
# Without prefix, treats as external localization files
# Path: Documents/Aottg2/CustomLocale/MyGameMode/English.json
# JSON file structure:
{
    "Name": "English",  // Required header
    "Hello": "World!",  // Localization values
    "Foo.Bar": "Baz"    // Localization values
}

Locale.RegisterLanguages("MyGameMode");

Game.Print("Hello: " + Locale.Get("Hello"));
Game.Print("Foo.Bar: " + Locale.Get("Foo.Bar"));

# Registering non-existing or empty localization files directory will throw an exception
Locale.RegisterLanguages("NonExistingGameMode");

# Set default fallback language (Russian instead of English)
Locale.DefaultLanguage = LanguageEnum.Russian;

# Fallback to default for missing key in current language
Locale.Set(LanguageEnum.Russian, "russian_key", "Сообщение");
Game.Print("russian_key: " + Locale.Get("russian_key"));

# Single-level (non-recursive) fallback: English -> German
Locale.RegisterFallback(LanguageEnum.English, LanguageEnum.German);
Locale.Set(LanguageEnum.German, "german_string", "Hallo");
Game.Print("german_string: " + Locale.Get("german_string"));

# By default Traditional Chinese falls back to Simplified Chinese
Locale.Set(LanguageEnum.Chinese, "chinese_string", "你好");
Game.Print("chinese_string: " + Locale.Get("chinese_string"));

# Clean up fallbacks
Locale.RemoveFallback(LanguageEnum.Chinese);
Locale.RemoveFallback(LanguageEnum.TraditionalChinese);

# Missing key throws an exception
Game.Print("missing_key: " + Locale.Get("missing_key"));
```
### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|CurrentLanguage|string|True|Returns the current language (e.g. "English" or "简体中文").|
|DefaultLanguage|string|False|The default language to use when a string is not found in the current language pack. English by default. Refer to [LanguageEnum](../Enums/LanguageEnum.md)|


### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Get(key: string) -> string</code></pre>
> Get the localized string for the given key. Searches the current UI language, then any registered fallbacks,
and finally the default language. Throws an exception if the key is not found in any language pack.
> 
> **Parameters**:
> - `key`: The key of the localized string to get.
> 
> **Returns**: The localized string.
<pre class="language-typescript"><code class="lang-typescript">function Set(language: string, key: string, value: string)</code></pre>
> Set or override a localized string for the specified language and key.
> 
> **Parameters**:
> - `language`: The language code. Refer to [LanguageEnum](../Enums/LanguageEnum.md)
> - `key`: The key of the localized string.
> - `value`: The localized string value.
> 
<pre class="language-typescript"><code class="lang-typescript">function RegisterLanguage(language: string, strings: <a data-footnote-ref href="#user-content-fn-1">Dict</a><string,string>)</code></pre>
> Register a single-level (non-recursive) fallback: if a string is not found in 'fromLanguage',
the system will search only in 'toLanguage', without chaining further.
> 
> **Parameters**:
> - `language`: The language code to register. Refer to [LanguageEnum](../Enums/LanguageEnum.md)
> - `strings`: The dictionary containing key-value pairs of localized strings.
> 
<pre class="language-typescript"><code class="lang-typescript">function RegisterLanguages(pattern: string)</code></pre>
> Register all localized strings from JSON files for a specific category across all available languages.
Use 'internal://' prefix for internal files (e.g., 'internal://BasicTutorialMap') or no prefix for external files (e.g., 'MyCustomMod').
> 
> **Parameters**:
> - `pattern`: The category pattern. Use 'internal://' prefix for internal files or no prefix for external files.
> 
<pre class="language-typescript"><code class="lang-typescript">function RegisterFallback(fromLanguage: string, toLanguage: string)</code></pre>
> Register a fallback language. When a string is not found in 'fromLanguage', it will try 'toLanguage'.
> 
> **Parameters**:
> - `fromLanguage`: The language code that will fallback to another language. Refer to [LanguageEnum](../Enums/LanguageEnum.md)
> - `toLanguage`: The language code to fallback to. Refer to [LanguageEnum](../Enums/LanguageEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function RemoveFallback(fromLanguage: string)</code></pre>
> Remove a language fallback.
> 
> **Parameters**:
> - `fromLanguage`: The language code to remove the fallback for. Refer to [LanguageEnum](../Enums/LanguageEnum.md)
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
