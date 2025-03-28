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
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetLabel</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">label</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">message</span>)
Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetLabelForTime</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">label</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">message</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">time</span>)
Sets the label for a certain time, after which it will be cleared.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetLabelAll</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">label</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">message</span>)
Sets the label for all players. Master client only. Be careful not to call this often.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetLabelForTimeAll</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">label</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">message</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">time</span>)
Sets the label for all players for a certain time. Master client only.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">CreatePopup</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">popupName</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">title</span>, <span style="color:#509cd4;">int</span> <span style="color:#9cdcfe;">width</span>, <span style="color:#509cd4;">int</span> <span style="color:#9cdcfe;">height</span>)
Creates a new popup. This popup is hidden until shown.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">ShowPopup</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">popupName</span>)
Shows the popup with given name.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">HidePopup</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">popupName</span>)
Hides the popup with given name.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">ClearPopup</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">popupName</span>)
Clears all elements in popup with given name.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">AddPopupLabel</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">popupName</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">label</span>)
Adds a text row to the popup with label as content.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">AddPopupButton</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">popupName</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">label</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">callback</span>)
Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">AddPopupBottomButton</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">popupName</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">label</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">callback</span>)
Adds a button to the bottom bar of the popup.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">AddPopupButtons</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">popupName</span>, <span style="color:#509cd4;">[List](../objects/List.md)</span> <span style="color:#9cdcfe;">labels</span>, <span style="color:#509cd4;">[List](../objects/List.md)</span> <span style="color:#9cdcfe;">callbacks</span>)
Adds a list of buttons in a row to the popup.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">WrapStyleTag</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">text</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">style</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">arg</span> = <span style="color:#509cd4;">null</span>)
Returns a wrapped string given style and args.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">GetLocale</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">cat</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">sub</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">key</span>)
Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.
#### <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#dcdcaa;">GetLanguage</span>()
Returns the current language (e.g. "English" or "简体中文").
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">ShowChangeCharacterMenu</span>()
Shows the change character menu if main character is Human.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetScoreboardHeader</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">header</span>)
Sets the display of the scoreboard header (default "Kills / Deaths...")
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetScoreboardProperty</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">property</span>)
Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.
#### <span style="color:#509cd4;">[Color](../objects/Color.md)</span> <span style="color:#dcdcaa;">GetThemeColor</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">panel</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">category</span>, <span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">item</span>)
Gets the color of the specified item. See theme json for reference.
#### <span style="color:#509cd4;">bool</span> <span style="color:#dcdcaa;">IsPopupActive</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">popupName</span>)
Returns if the given popup is active

---

