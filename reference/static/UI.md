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
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetLabel</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">label</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">message</mark>)
Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetLabelForTime</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">label</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">message</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">time</mark>)
Sets the label for a certain time, after which it will be cleared.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetLabelAll</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">label</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">message</mark>)
Sets the label for all players. Master client only. Be careful not to call this often.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetLabelForTimeAll</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">label</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">message</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">time</mark>)
Sets the label for all players for a certain time. Master client only.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">CreatePopup</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">popupName</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">title</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">width</mark>, <mark style="color:Blue;">int</mark> <mark style="color:Yellow;">height</mark>)
Creates a new popup. This popup is hidden until shown.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">ShowPopup</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">popupName</mark>)
Shows the popup with given name.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">HidePopup</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">popupName</mark>)
Hides the popup with given name.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">ClearPopup</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">popupName</mark>)
Clears all elements in popup with given name.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">AddPopupLabel</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">popupName</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">label</mark>)
Adds a text row to the popup with label as content.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">AddPopupButton</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">popupName</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">label</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">callback</mark>)
Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">AddPopupBottomButton</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">popupName</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">label</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">callback</mark>)
Adds a button to the bottom bar of the popup.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">AddPopupButtons</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">popupName</mark>, <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">labels</mark>, <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">callbacks</mark>)
Adds a list of buttons in a row to the popup.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">WrapStyleTag</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">text</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">style</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">arg</mark> = <mark style="color:Blue;">null</mark>)
Returns a wrapped string given style and args.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">GetLocale</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">cat</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">sub</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">key</mark>)
Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.
#### <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">GetLanguage</mark>()
Returns the current language (e.g. "English" or "简体中文").
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">ShowChangeCharacterMenu</mark>()
Shows the change character menu if main character is Human.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetScoreboardHeader</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">header</mark>)
Sets the display of the scoreboard header (default "Kills / Deaths...")
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetScoreboardProperty</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">property</mark>)
Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.
#### <mark style="color:Blue;">[Color](../objects/Color.md)</mark> <mark style="color:Yellow;">GetThemeColor</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">panel</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">category</mark>, <mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">item</mark>)
Gets the color of the specified item. See theme json for reference.
#### <mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">IsPopupActive</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">popupName</mark>)
Returns if the given popup is active

---

