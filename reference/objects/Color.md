# Color
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|R|int|False|Red component of the color|
|G|int|False|Green component of the color|
|B|int|False|Blue component of the color|
|A|int|False|Alpha component of the color|
## Methods
|Function|Returns|Description|
|---|---|---|
|ToHexString()|[String](../static/String.md)|Converts the color to a hex string|
## Static Methods
|Function|Returns|Description|
|---|---|---|
|Lerp(<br/>a : [Color](../objects/Color.md),<br/>b : [Color](../objects/Color.md),<br/>t : float<br/>)|[Color](../objects/Color.md)|Linearly interpolates between colors a and b by t|
|Gradient(<br/>a : [Color](../objects/Color.md),<br/>b : [Color](../objects/Color.md),<br/>t : float<br/>)|[Color](../objects/Color.md)|Creates a gradient color from two colors|
