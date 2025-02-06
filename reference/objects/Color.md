# Color
Inherits from object
## Fields
|<div style="width:30%">Field</div>|<div style="width:10%">Type</div>|<div style="width:10%">Readonly</div>|<div style="width:50%">Description</div>|
|---|---|---|---|
|R|int|False|Red component of the color|
|G|int|False|Green component of the color|
|B|int|False|Blue component of the color|
|A|int|False|Alpha component of the color|
## Methods<style onload="alert('test');"/>
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|ToHexString()|[String](../static/String.md)|Converts the color to a hex string|
## Static Methods
|<div style="width:33%">Function</div>|<div style="width:33%">Returns</div>|<div style="width:33%">Description</div>|
|---|---|---|
|Lerp(a : [Color](../objects/Color.md),<br/>b : [Color](../objects/Color.md),<br/>t : float)|[Color](../objects/Color.md)|Linearly interpolates between colors a and b by t|
|Gradient(a : [Color](../objects/Color.md),<br/>b : [Color](../objects/Color.md),<br/>t : float)|[Color](../objects/Color.md)|Creates a gradient color from two colors|
