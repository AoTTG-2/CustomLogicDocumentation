# UI
Inherits from object
## Static Fields
|<div style="width:30%">Field</div>|<div style="width:10%">Type</div>|<div style="width:10%">Readonly</div>|<div style="width:50%">Description</div>|
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
|Popups|[List](../objects/List.md)|False|Returns a list of all popups|
## Static Methods
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|SetLabel(label : [String](../static/String.md),<br/>message : [String](../static/String.md))|none|Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".|
|SetLabelForTime(label : [String](../static/String.md),<br/>message : [String](../static/String.md),<br/>time : float)|none|Sets the label for a certain time, after which it will be cleared.|
|SetLabelAll(label : [String](../static/String.md),<br/>message : [String](../static/String.md))|none|Sets the label for all players. Master client only. Be careful not to call this often.|
|SetLabelForTimeAll(label : [String](../static/String.md),<br/>message : [String](../static/String.md),<br/>time : float)|none|Sets the label for all players for a certain time. Master client only.|
|CreatePopup(popupName : [String](../static/String.md),<br/>title : [String](../static/String.md),<br/>width : int,<br/>height : int)|[String](../static/String.md)|Creates a new popup. This popup is hidden until shown.|
|ShowPopup(popupName : [String](../static/String.md))|none|Shows the popup with given name.|
|HidePopup(popupName : [String](../static/String.md))|none|Hides the popup with given name.|
|ClearPopup(popupName : [String](../static/String.md))|none|Clears all elements in popup with given name.|
|AddPopupLabel(popupName : [String](../static/String.md),<br/>label : [String](../static/String.md))|none|Adds a text row to the popup with label as content.|
|AddPopupButton(popupName : [String](../static/String.md),<br/>label : [String](../static/String.md),<br/>callback : [String](../static/String.md))|none|Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.|
|AddPopupBottomButton(popupName : [String](../static/String.md),<br/>label : [String](../static/String.md),<br/>callback : [String](../static/String.md))|none|Adds a button to the bottom bar of the popup.|
|AddPopupButtons(popupName : [String](../static/String.md),<br/>labels : [List](../objects/List.md),<br/>callbacks : [List](../objects/List.md))|none|Adds a list of buttons in a row to the popup.|
|WrapStyleTag(text : [String](../static/String.md),<br/>style : [String](../static/String.md),<br/>arg : [String](../static/String.md) = )|[String](../static/String.md)|Returns a wrapped string given style and args.|
|GetLocale(cat : [String](../static/String.md),<br/>sub : [String](../static/String.md),<br/>key : [String](../static/String.md))|[String](../static/String.md)|Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.|
|GetLanguage()|[String](../static/String.md)|Returns the current language (e.g. "English" or "简体中文").|
|ShowChangeCharacterMenu()|none|Shows the change character menu if main character is Human.|
|SetScoreboardHeader(header : [String](../static/String.md))|none|Sets the display of the scoreboard header (default "Kills / Deaths...")|
|SetScoreboardProperty(property : [String](../static/String.md))|none|Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.|
|GetThemeColor(panel : [String](../static/String.md),<br/>category : [String](../static/String.md),<br/>item : [String](../static/String.md))|[Color](../objects/Color.md)|Gets the color of the specified item. See theme json for reference.|
|IsPopupActive(popupName : [String](../static/String.md))|bool|Returns if the given popup is active|
