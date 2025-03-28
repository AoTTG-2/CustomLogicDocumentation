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
#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetLabel</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> label, <mark style="color:blue;">[String](../static/String.md)</mark> message)
> Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetLabelForTime</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> label, <mark style="color:blue;">[String](../static/String.md)</mark> message, <mark style="color:blue;">float</mark> time)
> Sets the label for a certain time, after which it will be cleared.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetLabelAll</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> label, <mark style="color:blue;">[String](../static/String.md)</mark> message)
> Sets the label for all players. Master client only. Be careful not to call this often.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetLabelForTimeAll</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> label, <mark style="color:blue;">[String](../static/String.md)</mark> message, <mark style="color:blue;">float</mark> time)
> Sets the label for all players for a certain time. Master client only.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">CreatePopup</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> popupName, <mark style="color:blue;">[String](../static/String.md)</mark> title, <mark style="color:blue;">int</mark> width, <mark style="color:blue;">int</mark> height)
> Creates a new popup. This popup is hidden until shown.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ShowPopup</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> popupName)
> Shows the popup with given name.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">HidePopup</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> popupName)
> Hides the popup with given name.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ClearPopup</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> popupName)
> Clears all elements in popup with given name.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">AddPopupLabel</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> popupName, <mark style="color:blue;">[String](../static/String.md)</mark> label)
> Adds a text row to the popup with label as content.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">AddPopupButton</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> popupName, <mark style="color:blue;">[String](../static/String.md)</mark> label, <mark style="color:blue;">[String](../static/String.md)</mark> callback)
> Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">AddPopupBottomButton</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> popupName, <mark style="color:blue;">[String](../static/String.md)</mark> label, <mark style="color:blue;">[String](../static/String.md)</mark> callback)
> Adds a button to the bottom bar of the popup.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">AddPopupButtons</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> popupName, <mark style="color:blue;">[List](../objects/List.md)</mark> labels, <mark style="color:blue;">[List](../objects/List.md)</mark> callbacks)
> Adds a list of buttons in a row to the popup.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">WrapStyleTag</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> text, <mark style="color:blue;">[String](../static/String.md)</mark> style, <mark style="color:blue;">[String](../static/String.md)</mark> arg = <mark style="color:blue;">null</mark>)
> Returns a wrapped string given style and args.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">GetLocale</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> cat, <mark style="color:blue;">[String](../static/String.md)</mark> sub, <mark style="color:blue;">[String](../static/String.md)</mark> key)
> Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.

#### <mark style="color:blue;">[String](../static/String.md)</mark> <mark style="color:yellow;">GetLanguage</mark>()
> Returns the current language (e.g. "English" or "简体中文").

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ShowChangeCharacterMenu</mark>()
> Shows the change character menu if main character is Human.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetScoreboardHeader</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> header)
> Sets the display of the scoreboard header (default "Kills / Deaths...")

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetScoreboardProperty</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> property)
> Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.

#### <mark style="color:blue;">[Color](../objects/Color.md)</mark> <mark style="color:yellow;">GetThemeColor</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> panel, <mark style="color:blue;">[String](../static/String.md)</mark> category, <mark style="color:blue;">[String](../static/String.md)</mark> item)
> Gets the color of the specified item. See theme json for reference.

#### <mark style="color:blue;">bool</mark> <mark style="color:yellow;">IsPopupActive</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> popupName)
> Returns if the given popup is active


---

