# LineRenderer
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|StartWidth|float|False|The width of the line at the start|
|EndWidth|float|False|The width of the line at the end|
|LineColor|[Color](../static/color.md)|False|The color of the line|
|PositionCount|int|False|The number of points in the line|
|Enabled|bool|False|Is the line renderer enabled|
|Loop|bool|False|Is the line renderer a loop|
|NumCornerVertices|int|False|The number of corner vertices|
|NumCapVertices|int|False|The number of end cap vertices|
|Alignment|[String](../static/string.md)|False|The alignment of the line renderer|
|TextureMode|[String](../static/string.md)|False|The texture mode of the line renderer|
|UseWorldSpace|bool|False|Is the line renderer in world space|
|ShadowCastingMode|[String](../static/string.md)|False|Does the line renderer cast shadows|
|ReceiveShadows|bool|False|Does the line renderer receive shadows|
|ColorGradient|[List](../objects/list.md)|False|The gradient of the line renderer|
|AlphaGradient|[List](../objects/list.md)|False|The alpha gradient of the line renderer|
|WidthCurve|[List](../objects/list.md)|False|The width curve of the line renderer|
|WidthMultiplier|float|False|The width multiplier of the line renderer|
|ColorGradientMode|[String](../static/string.md)|False|The color gradient mode of the line renderer|
## Methods
|Function|Returns|Description|
|---|---|---|
|CreateLineRenderer()|[LineRenderer](../static/linerenderer.md)|[Obselete] Create a new LineRenderer|
|GetPosition(index : int)|[Vector3](../static/vector3.md)|Get the position of a point in the line renderer|
|SetPosition(index : int, position : [Vector3](../static/vector3.md))|none|Set the position of a point in the line renderer|
