# UI
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Popups|[List](../objects/list.md)|False|Returns a list of all popups|
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|TopCenter|[String](../static/string.md)|False|"TopCenter" constant|
|TopLeft|[String](../static/string.md)|False|"TopLeft" constant|
|TopRight|[String](../static/string.md)|False|"TopRight" constant|
|MiddleCenter|[String](../static/string.md)|False|"MiddleCenter" constant|
|MiddleLeft|[String](../static/string.md)|False|"MiddleLeft" constant|
|MiddleRight|[String](../static/string.md)|False|"MiddleRight" constant|
|BottomCenter|[String](../static/string.md)|False|"BottomCenter" constant|
|BottomLeft|[String](../static/string.md)|False|"BottomLeft" constant|
|BottomRight|[String](../static/string.md)|False|"BottomRight" constant|
## Methods
|Function|Returns|Description|
|---|---|---|
|SetLabel(label : [String](../static/string.md), message : [String](../static/string.md))|none|Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".|
|SetLabelForTime(label : [String](../static/string.md), message : [String](../static/string.md), time : float)|none|Sets the label for a certain time, after which it will be cleared.|
|SetLabelAll(label : [String](../static/string.md), message : [String](../static/string.md))|none|Sets the label for all players. Master client only. Be careful not to call this often.|
|SetLabelForTimeAll(label : [String](../static/string.md), message : [String](../static/string.md), time : float)|none|Sets the label for all players for a certain time. Master client only.|
|CreatePopup(popupName : [String](../static/string.md), title : [String](../static/string.md), width : int, height : int)|[String](../static/string.md)|Creates a new popup. This popup is hidden until shown.|
|ShowPopup(popupName : [String](../static/string.md))|none|Shows the popup with given name.|
|HidePopup(popupName : [String](../static/string.md))|none|Hides the popup with given name.|
|ClearPopup(popupName : [String](../static/string.md))|none|Clears all elements in popup with given name.|
|AddPopupLabel(popupName : [String](../static/string.md), label : [String](../static/string.md))|none|Adds a text row to the popup with label as content.|
|AddPopupButton(popupName : [String](../static/string.md), label : [String](../static/string.md), callback : [String](../static/string.md))|none|Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.|
|AddPopupBottomButton(popupName : [String](../static/string.md), label : [String](../static/string.md), callback : [String](../static/string.md))|none|Adds a button to the bottom bar of the popup.|
|AddPopupButtons(popupName : [String](../static/string.md), labels : [List](../objects/list.md), callbacks : [List](../objects/list.md))|none|Adds a list of buttons in a row to the popup.|
|WrapStyleTag(text : [String](../static/string.md), style : [String](../static/string.md), arg : [String](../static/string.md) = )|[String](../static/string.md)|Returns a wrapped string given style and args.|
|GetLocale(cat : [String](../static/string.md), sub : [String](../static/string.md), key : [String](../static/string.md))|[String](../static/string.md)|Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.|
|GetLanguage()|[String](../static/string.md)|Returns the current language (e.g. "English" or "简体中文").|
|ShowChangeCharacterMenu()|none|Shows the change character menu if main character is Human.|
|SetScoreboardHeader(header : [String](../static/string.md))|none|Sets the display of the scoreboard header (default "Kills / Deaths...")|
|SetScoreboardProperty(property : [String](../static/string.md))|none|Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.|
|GetThemeColor(panel : [String](../static/string.md), category : [String](../static/string.md), item : [String](../static/string.md))|[Color](../static/color.md)|Gets the color of the specified item. See theme json for reference.|
|IsPopupActive(popupName : [String](../static/string.md))|bool|Returns if the given popup is active|
