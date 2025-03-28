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
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetLabel</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">label</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">message</mark>)
Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetLabelForTime</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">label</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">message</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">time</mark>)
Sets the label for a certain time, after which it will be cleared.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetLabelAll</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">label</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">message</mark>)
Sets the label for all players. Master client only. Be careful not to call this often.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetLabelForTimeAll</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">label</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">message</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">time</mark>)
Sets the label for all players for a certain time. Master client only.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">CreatePopup</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">popupName</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">title</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">width</mark>, <mark style="color:#509cd4;">int</mark> <mark style="color:#9cdcfe;">height</mark>)
Creates a new popup. This popup is hidden until shown.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ShowPopup</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">popupName</mark>)
Shows the popup with given name.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">HidePopup</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">popupName</mark>)
Hides the popup with given name.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ClearPopup</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">popupName</mark>)
Clears all elements in popup with given name.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">AddPopupLabel</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">popupName</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">label</mark>)
Adds a text row to the popup with label as content.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">AddPopupButton</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">popupName</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">label</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">callback</mark>)
Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">AddPopupBottomButton</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">popupName</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">label</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">callback</mark>)
Adds a button to the bottom bar of the popup.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">AddPopupButtons</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">popupName</mark>, <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#9cdcfe;">labels</mark>, <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#9cdcfe;">callbacks</mark>)
Adds a list of buttons in a row to the popup.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">WrapStyleTag</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">text</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">style</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">arg</mark> = <mark style="color:#509cd4;">null</mark>)
Returns a wrapped string given style and args.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">GetLocale</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">cat</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">sub</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">key</mark>)
Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.
#### <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#dcdcaa;">GetLanguage</mark>()
Returns the current language (e.g. "English" or "简体中文").
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ShowChangeCharacterMenu</mark>()
Shows the change character menu if main character is Human.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetScoreboardHeader</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">header</mark>)
Sets the display of the scoreboard header (default "Kills / Deaths...")
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetScoreboardProperty</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">property</mark>)
Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.
#### <mark style="color:#509cd4;">[Color](../objects/Color.md)</mark> <mark style="color:#dcdcaa;">GetThemeColor</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">panel</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">category</mark>, <mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">item</mark>)
Gets the color of the specified item. See theme json for reference.
#### <mark style="color:#509cd4;">bool</mark> <mark style="color:#dcdcaa;">IsPopupActive</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">popupName</mark>)
Returns if the given popup is active

---

