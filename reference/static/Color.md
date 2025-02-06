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
|Lerp(a : [Color](../static/Color.md), b : [Color](../static/Color.md), t : float)|[Color](../static/Color.md)|Linearly interpolates between colors a and b by t|
|Gradient(a : [Color](../static/Color.md), b : [Color](../static/Color.md), t : float)|[Color](../static/Color.md)|Creates a gradient color from two colors|
