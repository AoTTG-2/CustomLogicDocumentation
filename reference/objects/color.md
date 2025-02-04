# Color

Inherits from Object. Is a struct, meaning that assignments will create copies and comparisons will return true if all fields are equivalent.

### Initialization

Color takes four ints R, G, B, and A as parameters when initializing. Values are between 0 and 255.

```python
# create a 255,255,255,255 color
color = Color();

# create a 128,56,48,255 color
color = Color(128, 56, 48);

# create a 128, 56, 48, 128 color
color = Color(128, 56, 48, 128);

# create a color from hex string
color = Color("#FF0000");
```

### Fields

<table><thead><tr><th width="175.33333333333331">Field</th><th width="99">Type</th><th width="103">Readonly</th><th>Description</th></tr></thead><tbody><tr><td>R</td><td>int</td><td>false</td><td>Red</td></tr><tr><td>G</td><td>int</td><td>false</td><td>Green</td></tr><tr><td>B</td><td>int</td><td>false</td><td>Blue</td></tr><tr><td>A</td><td>int</td><td>false</td><td>Alpha</td></tr></tbody></table>

### Functions

<table><thead><tr><th width="263.3333333333333">Function</th><th width="94">Returns</th><th>Description</th></tr></thead><tbody><tr><td>ToHexString()</td><td>string</td><td>Converts the color to a hex string</td></tr><tr><td>Gradient(a: Color, b: Color, fade: float)</td><td>Color</td><td>Returns a gradient color between a and b using the fade value.</td></tr></tbody></table>
