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
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetLabel</span>(<span style="color:blue;">[String](../static/String.md)</span> label, <span style="color:blue;">[String](../static/String.md)</span> message)
> Sets the label at a certain location. Valid types: "TopCenter", "TopLeft", "TopRight", "MiddleCenter", "MiddleLeft", "MiddleRight", "BottomLeft", "BottomRight", "BottomCenter".
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetLabelForTime</span>(<span style="color:blue;">[String](../static/String.md)</span> label, <span style="color:blue;">[String](../static/String.md)</span> message, <span style="color:blue;">float</span> time)
> Sets the label for a certain time, after which it will be cleared.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetLabelAll</span>(<span style="color:blue;">[String](../static/String.md)</span> label, <span style="color:blue;">[String](../static/String.md)</span> message)
> Sets the label for all players. Master client only. Be careful not to call this often.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetLabelForTimeAll</span>(<span style="color:blue;">[String](../static/String.md)</span> label, <span style="color:blue;">[String](../static/String.md)</span> message, <span style="color:blue;">float</span> time)
> Sets the label for all players for a certain time. Master client only.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">CreatePopup</span>(<span style="color:blue;">[String](../static/String.md)</span> popupName, <span style="color:blue;">[String](../static/String.md)</span> title, <span style="color:blue;">int</span> width, <span style="color:blue;">int</span> height)
> Creates a new popup. This popup is hidden until shown.
#### <span style="color:blue;">void</span> <span style="color:yellow;">ShowPopup</span>(<span style="color:blue;">[String](../static/String.md)</span> popupName)
> Shows the popup with given name.
#### <span style="color:blue;">void</span> <span style="color:yellow;">HidePopup</span>(<span style="color:blue;">[String](../static/String.md)</span> popupName)
> Hides the popup with given name.
#### <span style="color:blue;">void</span> <span style="color:yellow;">ClearPopup</span>(<span style="color:blue;">[String](../static/String.md)</span> popupName)
> Clears all elements in popup with given name.
#### <span style="color:blue;">void</span> <span style="color:yellow;">AddPopupLabel</span>(<span style="color:blue;">[String](../static/String.md)</span> popupName, <span style="color:blue;">[String](../static/String.md)</span> label)
> Adds a text row to the popup with label as content.
#### <span style="color:blue;">void</span> <span style="color:yellow;">AddPopupButton</span>(<span style="color:blue;">[String](../static/String.md)</span> popupName, <span style="color:blue;">[String](../static/String.md)</span> label, <span style="color:blue;">[String](../static/String.md)</span> callback)
> Adds a button row to the popup with given button name and display text. When button is pressed, OnButtonClick is called in Main with buttonName parameter.
#### <span style="color:blue;">void</span> <span style="color:yellow;">AddPopupBottomButton</span>(<span style="color:blue;">[String](../static/String.md)</span> popupName, <span style="color:blue;">[String](../static/String.md)</span> label, <span style="color:blue;">[String](../static/String.md)</span> callback)
> Adds a button to the bottom bar of the popup.
#### <span style="color:blue;">void</span> <span style="color:yellow;">AddPopupButtons</span>(<span style="color:blue;">[String](../static/String.md)</span> popupName, <span style="color:blue;">[List](../objects/List.md)</span> labels, <span style="color:blue;">[List](../objects/List.md)</span> callbacks)
> Adds a list of buttons in a row to the popup.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">WrapStyleTag</span>(<span style="color:blue;">[String](../static/String.md)</span> text, <span style="color:blue;">[String](../static/String.md)</span> style, <span style="color:blue;">[String](../static/String.md)</span> arg = <span style="color:blue;">null</span>)
> Returns a wrapped string given style and args.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">GetLocale</span>(<span style="color:blue;">[String](../static/String.md)</span> cat, <span style="color:blue;">[String](../static/String.md)</span> sub, <span style="color:blue;">[String](../static/String.md)</span> key)
> Gets translated locale from the current Language.json file with given category, subcategory, and key pattern.
#### <span style="color:blue;">[String](../static/String.md)</span> <span style="color:yellow;">GetLanguage</span>()
> Returns the current language (e.g. "English" or "简体中文").
#### <span style="color:blue;">void</span> <span style="color:yellow;">ShowChangeCharacterMenu</span>()
> Shows the change character menu if main character is Human.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetScoreboardHeader</span>(<span style="color:blue;">[String](../static/String.md)</span> header)
> Sets the display of the scoreboard header (default "Kills / Deaths...")
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetScoreboardProperty</span>(<span style="color:blue;">[String](../static/String.md)</span> property)
> Sets which Player custom property to read from to display on the scoreboard. If set to empty string, will use the default "Kills / Deaths..." display.
#### <span style="color:blue;">[Color](../objects/Color.md)</span> <span style="color:yellow;">GetThemeColor</span>(<span style="color:blue;">[String](../static/String.md)</span> panel, <span style="color:blue;">[String](../static/String.md)</span> category, <span style="color:blue;">[String](../static/String.md)</span> item)
> Gets the color of the specified item. See theme json for reference.
#### <span style="color:blue;">bool</span> <span style="color:yellow;">IsPopupActive</span>(<span style="color:blue;">[String](../static/String.md)</span> popupName)
> Returns if the given popup is active

---

