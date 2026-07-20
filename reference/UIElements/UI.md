# UI
Inherits from [Object](../objects/Object.md)

UI label functions.

### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|ForceHideNames|bool|False|Gets or sets whether character info popups should be force hidden. When enabled, character names will be hidden regardless of popup state. This is useful for custom UI panels that should hide character names when active. If this is enabled and then disabled, normal popup behavior resumes.|
|GetPopups|[List](../Collections/List.md)<string>|True|Returns a list of all popups.|


### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function SetLabel(label: string, message: string)</code></pre>
> Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight",
"MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".
> 
> **Parameters**:
> - `label`: The label location. Refer to [UILabelEnum](../Enums/UILabelEnum.md)
> - `message`: The message to display.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetLabelForTime(label: string, message: string, time: float)</code></pre>
> Sets the label for a certain time, after which it will be cleared.
> 
> **Parameters**:
> - `label`: The label location. Refer to [UILabelEnum](../Enums/UILabelEnum.md)
> - `message`: The message to display.
> - `time`: The time in seconds before the label is cleared.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetLabelAll(label: string, message: string)</code></pre>
> Sets the label for all players. Master client only. Be careful not to call this often.
> 
> **Parameters**:
> - `label`: The label location. Refer to [UILabelEnum](../Enums/UILabelEnum.md)
> - `message`: The message to display.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetLabelForTimeAll(label: string, message: string, time: float)</code></pre>
> Sets the label for all players for a certain time. Master client only.
> 
> **Parameters**:
> - `label`: The label location.
> - `message`: The message to display.
> - `time`: The time in seconds before the label is cleared.
> 
<pre class="language-typescript"><code class="lang-typescript">function CreatePopup(popupName: string, title: string, width: int, height: int) -> string</code></pre>
> Creates a new popup. This popup is hidden until shown.
> 
> **Parameters**:
> - `popupName`: The name of the popup.
> - `title`: The title of the popup.
> - `width`: The width of the popup.
> - `height`: The height of the popup.
> 
> **Returns**: The popup name.
<pre class="language-typescript"><code class="lang-typescript">function ShowPopup(popupName: string)</code></pre>
> Shows the popup with given name.
> 
> **Parameters**:
> - `popupName`: The name of the popup to show.
> 
<pre class="language-typescript"><code class="lang-typescript">function HidePopup(popupName: string)</code></pre>
> Hides the popup with given name.
> 
> **Parameters**:
> - `popupName`: The name of the popup to hide.
> 
<pre class="language-typescript"><code class="lang-typescript">function ClearPopup(popupName: string)</code></pre>
> Clears all elements in popup with given name.
> 
> **Parameters**:
> - `popupName`: The name of the popup to clear.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddPopupLabel(popupName: string, label: string)</code></pre>
> Adds a text row to the popup with label as content.
> 
> **Parameters**:
> - `popupName`: The name of the popup.
> - `label`: The label text to add.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddPopupButton(popupName: string, label: string, callback: string)</code></pre>
> Adds a button row to the popup with given button name and display text.
When button is pressed, OnButtonClick is called in Main with buttonName parameter.
> 
> **Parameters**:
> - `popupName`: The name of the popup.
> - `label`: The button display text.
> - `callback`: The callback name that will be passed to OnButtonClick in Main.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddPopupBottomButton(popupName: string, label: string, callback: string)</code></pre>
> Adds a button to the bottom bar of the popup.
> 
> **Parameters**:
> - `popupName`: The name of the popup.
> - `label`: The button display text.
> - `callback`: The callback name that will be passed to OnButtonClick in Main.
> 
<pre class="language-typescript"><code class="lang-typescript">function AddPopupButtons(popupName: string, labels: <a data-footnote-ref href="#user-content-fn-3">List</a><string>, callbacks: <a data-footnote-ref href="#user-content-fn-3">List</a><void>)</code></pre>
> Adds a list of buttons in a row to the popup.
> 
> **Parameters**:
> - `popupName`: The name of the popup.
> - `labels`: List of button display texts.
> - `callbacks`: List of callback names that will be passed to OnButtonClick in Main.
> 
<pre class="language-typescript"><code class="lang-typescript">function WrapStyleTag(text: string, style: string, arg: string = null) -> string</code></pre>
> Returns a wrapped string given style and args.
> 
> **Parameters**:
> - `text`: The text to wrap.
> - `style`: The style tag name.
> - `arg`: Optional style argument.
> 
> **Returns**: The wrapped string.
<pre class="language-typescript"><code class="lang-typescript">function ShowChangeCharacterMenu()</code></pre>
> Shows the change character menu if main character is Human.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetScoreboardHeader(header: string)</code></pre>
> Sets the display of the scoreboard header (default "Kills / Deaths...").
> 
> **Parameters**:
> - `header`: The header text to display.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetScoreboardProperty(property: string)</code></pre>
> Sets which Player custom property to read from to display on the scoreboard.
If set to empty string, will use the default "Kills / Deaths..." display.
> 
> **Parameters**:
> - `property`: The property name to read from Player custom properties.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetThemeColor(panel: string, category: string, item: string) -> <a data-footnote-ref href="#user-content-fn-0">Color</a></code></pre>
> Gets the color of the specified item. See theme json for reference.
> 
> **Parameters**:
> - `panel`: The panel name.
> - `category`: The category name.
> - `item`: The item name.
> 
> **Returns**: The theme color.
<pre class="language-typescript"><code class="lang-typescript">function IsPopupActive(popupName: string) -> bool</code></pre>
> Returns if the given popup is active.
> 
> **Parameters**:
> - `popupName`: The name of the popup to check.
> 
> **Returns**: True if the popup is active, false otherwise.
<pre class="language-typescript"><code class="lang-typescript">function SetLabelActive(label: string, active: bool)</code></pre>
> Sets whether a label is active or not.
> 
> **Parameters**:
> - `label`: The label name.
> - `active`: Whether the label should be active.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetKDRPanelActive(active: bool)</code></pre>
> Sets whether the KDR panel (top-left) is active or not.
> 
> **Parameters**:
> - `active`: Whether the KDR panel should be active.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetMinimapActive(active: bool)</code></pre>
> Sets whether the minimap is active or not.
> 
> **Parameters**:
> - `active`: Whether the minimap should be active.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetChatPanelActive(active: bool)</code></pre>
> Sets whether the chat panel is active or not.
> 
> **Parameters**:
> - `active`: Whether the chat panel should be active.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetFeedPanelActive(active: bool)</code></pre>
> Sets whether the feed panel is active or not.
> 
> **Parameters**:
> - `active`: Whether the feed panel should be active.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetBottomHUDActive(active: bool)</code></pre>
> Sets whether the bottom HUD is active or not. This can only be used when the character is alive.
> 
> **Parameters**:
> - `active`: Whether the bottom HUD should be active.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetRootVisualElement() -> <a data-footnote-ref href="#user-content-fn-118">VisualElement</a></code></pre>
> Returns the root `VisualElement` which you can add other elements to.
> 
> **Returns**: The root `VisualElement`.
<pre class="language-typescript"><code class="lang-typescript">function VisualElement() -> <a data-footnote-ref href="#user-content-fn-118">VisualElement</a></code></pre>
> Creates a new `VisualElement`.
> 
> **Returns**: A new VisualElement.
<pre class="language-typescript"><code class="lang-typescript">function Button(text: string = "", clickEvent: function = null) -> <a data-footnote-ref href="#user-content-fn-107">Button</a></code></pre>
> Creates a new `Button` with optional text and click event.
> 
> **Parameters**:
> - `text`: The text that the button displays.
> - `clickEvent`: The function that will be called when button is clicked.
> 
> **Returns**: A new Button.
<pre class="language-typescript"><code class="lang-typescript">function Label(text: string = "") -> <a data-footnote-ref href="#user-content-fn-111">Label</a></code></pre>
> Creates a new `Label` with optional text.
> 
> **Parameters**:
> - `text`: The text to be displayed.
> 
> **Returns**: A new Label.
<pre class="language-typescript"><code class="lang-typescript">function TextField(label: string = "") -> <a data-footnote-ref href="#user-content-fn-115">TextField</a></code></pre>
> Creates a new `TextField` with optional label.
> 
> **Parameters**:
> - `label`: The label text displayed next to the TextField (default: empty).
> 
> **Returns**: A new TextField.
<pre class="language-typescript"><code class="lang-typescript">function Toggle(label: string = "", valueChangedEvent: function = null) -> <a data-footnote-ref href="#user-content-fn-116">Toggle</a></code></pre>
> Creates a new `Toggle` with optional label and value changed event.
> 
> **Parameters**:
> - `label`: The label text displayed next to the toggle.
> - `valueChangedEvent`: The function that will be called when toggle value changes.
> 
> **Returns**: A new Toggle.
<pre class="language-typescript"><code class="lang-typescript">function Slider(lowValue: float = 0, highValue: float = 100, tickInterval: float = 0, label: string = "", valueChangedEvent: function = null) -> <a data-footnote-ref href="#user-content-fn-114">Slider</a></code></pre>
> Creates a new `Slider` for floating-point values with optional range, tick interval, and value changed event.
The slider will snap to values at multiples of the tick interval.
> 
> **Parameters**:
> - `lowValue`: The minimum value of the slider.
> - `highValue`: The maximum value of the slider.
> - `tickInterval`: The interval between allowed values. If 0, no snapping occurs. For example, 0.1 will snap to 0.0, 0.1, 0.2, etc.
> - `label`: The label text displayed next to the slider.
> - `valueChangedEvent`: The function that will be called when slider value changes.
> 
> **Returns**: A new Slider.
<pre class="language-typescript"><code class="lang-typescript">function SliderInt(lowValue: int = 0, highValue: int = 100, tickInterval: int = 1, label: string = "", valueChangedEvent: function = null) -> <a data-footnote-ref href="#user-content-fn-114">Slider</a></code></pre>
> Creates a new `Slider` for integer values with optional range, tick interval, and value changed event.
The slider will snap to values at multiples of the tick interval.
> 
> **Parameters**:
> - `lowValue`: The minimum value of the slider.
> - `highValue`: The maximum value of the slider.
> - `tickInterval`: The interval between allowed values. For example, 5 will snap to 0, 5, 10, 15, etc.
> - `label`: The label text displayed next to the slider.
> - `valueChangedEvent`: The function that will be called when slider value changes.
> 
> **Returns**: A new SliderInt.
<pre class="language-typescript"><code class="lang-typescript">function Dropdown(choices: <a data-footnote-ref href="#user-content-fn-3">List</a><string>, defaultIndex: int = 0, label: string = "", valueChangedEvent: function = null) -> <a data-footnote-ref href="#user-content-fn-108">Dropdown</a></code></pre>
> Creates a new `Dropdown` with a list of choices and optional label and value changed event.
> 
> **Parameters**:
> - `choices`: List of string options to display in the dropdown.
> - `defaultIndex`: The index of the initially selected option (default: 0).
> - `label`: The label text displayed next to the dropdown.
> - `valueChangedEvent`: The function that will be called when dropdown value changes.
> 
> **Returns**: A new Dropdown.
<pre class="language-typescript"><code class="lang-typescript">function ProgressBar(lowValue: float = 0, highValue: float = 100, title: string = "", valueChangedEvent: function = null) -> <a data-footnote-ref href="#user-content-fn-112">ProgressBar</a></code></pre>
> Creates a new `ProgressBar` with optional range, title, and value changed event.
> 
> **Parameters**:
> - `lowValue`: The minimum value of the progress bar (default: 0).
> - `highValue`: The maximum value of the progress bar (default: 100).
> - `title`: The title text displayed on the progress bar.
> - `valueChangedEvent`: The function that will be called when progress bar value changes.
> 
> **Returns**: A new ProgressBar.
<pre class="language-typescript"><code class="lang-typescript">function ScrollView() -> <a data-footnote-ref href="#user-content-fn-113">ScrollView</a></code></pre>
> Creates a new `ScrollView` for scrollable content.
> 
> **Returns**: A new ScrollView.
<pre class="language-typescript"><code class="lang-typescript">function Icon(iconPath: string = "") -> <a data-footnote-ref href="#user-content-fn-109">Icon</a></code></pre>
> Creates a new `Icon` element for displaying images/icons.
> 
> **Parameters**:
> - `iconPath`: Path to the icon resource (e.g., "Icons/Game/BladeIcon").
> 
> **Returns**: A new Icon.
<pre class="language-typescript"><code class="lang-typescript">function Image(iconPath: string = "") -> <a data-footnote-ref href="#user-content-fn-110">Image</a></code></pre>
> Creates a new `Image` element for displaying images/icons.
> 
> **Parameters**:
> - `iconPath`: Path to the icon resource (e.g., "Icons/Game/BladeIcon").
> 
> **Returns**: A new Image.

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
