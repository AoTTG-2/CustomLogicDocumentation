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
|Popups|[List](../objects/List.md)|False|Returns a list of all popups|
## Static Methods
|Function|Returns|Description|
|---|---|---|
|SetLabel(<br/><i>label</i> : [String](../static/String.md),<br/><i>message</i> : [String](../static/String.md)<br/>)|none|Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".|
|SetLabelForTime(<br/><i>label</i> : [String](../static/String.md),<br/><i>message</i> : [String](../static/String.md),<br/><i>time</i> : float<br/>)|none|Sets the label for a certain time, after which it will be cleared.|
|SetLabelAll(<br/><i>label</i> : [String](../static/String.md),<br/><i>message</i> : [String](../static/String.md)<br/>)|none|Sets the label for all players. Master client only. Be careful not to call this often.|
|SetLabelForTimeAll(<br/><i>label</i> : [String](../static/String.md),<br/><i>message</i> : [String](../static/String.md),<br/><i>time</i> : float<br/>)|none|Sets the label for all players for a certain time. Master client only.|
|CreatePopup(<br/><i>popupName</i> : [String](../static/String.md),<br/><i>title</i> : [String](../static/String.md),<br/><i>width</i> : int,<br/><i>height</i> : int<br/>)|[String](../static/String.md)|Creates a new popup. This popup is hidden until shown.|
|ShowPopup(<i>popupName</i> : [String](../static/String.md))|none|Shows the popup with given name.|
|HidePopup(<i>popupName</i> : [String](../static/String.md))|none|Hides the popup with given name.|
|ClearPopup(<i>popupName</i> : [String](../static/String.md))|none|Clears all elements in popup with given name.|
|AddPopupLabel(<br/><i>popupName</i> : [String](../static/String.md),<br/><i>label</i> : [String](../static/String.md)<br/>)|none|Adds a text row to the popup with label as content.|
|AddPopupButton(<br/><i>popupName</i> : [String](../static/String.md),<br/><i>label</i> : [String](../static/String.md),<br/><i>callback</i> : [String](../static/String.md)<br/>)|none|Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.|
|AddPopupBottomButton(<br/><i>popupName</i> : [String](../static/String.md),<br/><i>label</i> : [String](../static/String.md),<br/><i>callback</i> : [String](../static/String.md)<br/>)|none|Adds a button to the bottom bar of the popup.|
|AddPopupButtons(<br/><i>popupName</i> : [String](../static/String.md),<br/><i>labels</i> : [List](../objects/List.md),<br/><i>callbacks</i> : [List](../objects/List.md)<br/>)|none|Adds a list of buttons in a row to the popup.|
|WrapStyleTag(<br/><i>text</i> : [String](../static/String.md),<br/><i>style</i> : [String](../static/String.md),<br/><i>arg</i> : [String](../static/String.md) = <br/>)|[String](../static/String.md)|Returns a wrapped string given style and args.|
|GetLocale(<br/><i>cat</i> : [String](../static/String.md),<br/><i>sub</i> : [String](../static/String.md),<br/><i>key</i> : [String](../static/String.md)<br/>)|[String](../static/String.md)|Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.|
|GetLanguage()|[String](../static/String.md)|Returns the current language (e.g. "English" or "简体中文").|
|ShowChangeCharacterMenu()|none|Shows the change character menu if main character is Human.|
|SetScoreboardHeader(<i>header</i> : [String](../static/String.md))|none|Sets the display of the scoreboard header (default "Kills / Deaths...")|
|SetScoreboardProperty(<i>property</i> : [String](../static/String.md))|none|Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.|
|GetThemeColor(<br/><i>panel</i> : [String](../static/String.md),<br/><i>category</i> : [String](../static/String.md),<br/><i>item</i> : [String](../static/String.md)<br/>)|[Color](../objects/Color.md)|Gets the color of the specified item. See theme json for reference.|
|IsPopupActive(<i>popupName</i> : [String](../static/String.md))|bool|Returns if the given popup is active|
