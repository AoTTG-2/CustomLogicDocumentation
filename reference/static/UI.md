# UI
Inherits from object
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|TopCenter|[String](../static/String.md)|False|"TopCenter" constant|
|TopLeft|[String](../static/String.md)|False|"TopLeft" constant|
|TopRight|[String](../static/String.md)|False|"TopRight" constant|
|MiddleCenter|[String](../static/String.md)|False|"MiddleCenter" constant|
|MiddleLeft|[String](../static/String.md)|False|"MiddleLeft" constant|
|MiddleRight|[String](../static/String.md)|False|"MiddleRight" constant|
|BottomCenter|[String](../static/String.md)|False|"BottomCenter" constant|
|BottomLeft|[String](../static/String.md)|False|"BottomLeft" constant|
|BottomRight|[String](../static/String.md)|False|"BottomRight" constant|
|GetPopups|[List](../objects/List.md)|False|Returns a list of all popups|
## Static Methods
#### void <span style="color":#dcdcaa>SetLabel<span>([String](../static/String.md) <span style="color":#9cdcfe>label<span>, [String](../static/String.md) <span style="color":#9cdcfe>message<span>)
Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".
#### void <span style="color":#dcdcaa>SetLabelForTime<span>([String](../static/String.md) <span style="color":#9cdcfe>label<span>, [String](../static/String.md) <span style="color":#9cdcfe>message<span>, float <span style="color":#9cdcfe>time<span>)
Sets the label for a certain time, after which it will be cleared.
#### void <span style="color":#dcdcaa>SetLabelAll<span>([String](../static/String.md) <span style="color":#9cdcfe>label<span>, [String](../static/String.md) <span style="color":#9cdcfe>message<span>)
Sets the label for all players. Master client only. Be careful not to call this often.
#### void <span style="color":#dcdcaa>SetLabelForTimeAll<span>([String](../static/String.md) <span style="color":#9cdcfe>label<span>, [String](../static/String.md) <span style="color":#9cdcfe>message<span>, float <span style="color":#9cdcfe>time<span>)
Sets the label for all players for a certain time. Master client only.
#### [String](../static/String.md) <span style="color":#dcdcaa>CreatePopup<span>([String](../static/String.md) <span style="color":#9cdcfe>popupName<span>, [String](../static/String.md) <span style="color":#9cdcfe>title<span>, int <span style="color":#9cdcfe>width<span>, int <span style="color":#9cdcfe>height<span>)
Creates a new popup. This popup is hidden until shown.
#### void <span style="color":#dcdcaa>ShowPopup<span>([String](../static/String.md) <span style="color":#9cdcfe>popupName<span>)
Shows the popup with given name.
#### void <span style="color":#dcdcaa>HidePopup<span>([String](../static/String.md) <span style="color":#9cdcfe>popupName<span>)
Hides the popup with given name.
#### void <span style="color":#dcdcaa>ClearPopup<span>([String](../static/String.md) <span style="color":#9cdcfe>popupName<span>)
Clears all elements in popup with given name.
#### void <span style="color":#dcdcaa>AddPopupLabel<span>([String](../static/String.md) <span style="color":#9cdcfe>popupName<span>, [String](../static/String.md) <span style="color":#9cdcfe>label<span>)
Adds a text row to the popup with label as content.
#### void <span style="color":#dcdcaa>AddPopupButton<span>([String](../static/String.md) <span style="color":#9cdcfe>popupName<span>, [String](../static/String.md) <span style="color":#9cdcfe>label<span>, [String](../static/String.md) <span style="color":#9cdcfe>callback<span>)
Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.
#### void <span style="color":#dcdcaa>AddPopupBottomButton<span>([String](../static/String.md) <span style="color":#9cdcfe>popupName<span>, [String](../static/String.md) <span style="color":#9cdcfe>label<span>, [String](../static/String.md) <span style="color":#9cdcfe>callback<span>)
Adds a button to the bottom bar of the popup.
#### void <span style="color":#dcdcaa>AddPopupButtons<span>([String](../static/String.md) <span style="color":#9cdcfe>popupName<span>, [List](../objects/List.md) <span style="color":#9cdcfe>labels<span>, [List](../objects/List.md) <span style="color":#9cdcfe>callbacks<span>)
Adds a list of buttons in a row to the popup.
#### [String](../static/String.md) <span style="color":#dcdcaa>WrapStyleTag<span>([String](../static/String.md) <span style="color":#9cdcfe>text<span>, [String](../static/String.md) <span style="color":#9cdcfe>style<span>, [String](../static/String.md) <span style="color":#9cdcfe>arg<span> = null)
Returns a wrapped string given style and args.
#### [String](../static/String.md) <span style="color":#dcdcaa>GetLocale<span>([String](../static/String.md) <span style="color":#9cdcfe>cat<span>, [String](../static/String.md) <span style="color":#9cdcfe>sub<span>, [String](../static/String.md) <span style="color":#9cdcfe>key<span>)
Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.
#### [String](../static/String.md) <span style="color":#dcdcaa>GetLanguage<span>()
Returns the current language (e.g. "English" or "简体中文").
#### void <span style="color":#dcdcaa>ShowChangeCharacterMenu<span>()
Shows the change character menu if main character is Human.
#### void <span style="color":#dcdcaa>SetScoreboardHeader<span>([String](../static/String.md) <span style="color":#9cdcfe>header<span>)
Sets the display of the scoreboard header (default "Kills / Deaths...")
#### void <span style="color":#dcdcaa>SetScoreboardProperty<span>([String](../static/String.md) <span style="color":#9cdcfe>property<span>)
Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.
#### [Color](../objects/Color.md) <span style="color":#dcdcaa>GetThemeColor<span>([String](../static/String.md) <span style="color":#9cdcfe>panel<span>, [String](../static/String.md) <span style="color":#9cdcfe>category<span>, [String](../static/String.md) <span style="color":#9cdcfe>item<span>)
Gets the color of the specified item. See theme json for reference.
#### bool <span style="color":#dcdcaa>IsPopupActive<span>([String](../static/String.md) <span style="color":#9cdcfe>popupName<span>)
Returns if the given popup is active

---

