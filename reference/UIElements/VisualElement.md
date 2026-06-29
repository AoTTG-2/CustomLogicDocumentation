# VisualElement
Inherits from [Object](../objects/Object.md)

Base class for all UI elements. Note: Most methods return self to allow method chaining.

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|ChildCount|int|True|The number of child elements in this visual element.|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Add(visualElement: <a data-footnote-ref href="#user-content-fn-116">VisualElement</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Add a child element.
> 
> **Parameters**:
> - `visualElement`: The visual element to add as a child.
> 
<pre class="language-typescript"><code class="lang-typescript">function Remove(visualElement: <a data-footnote-ref href="#user-content-fn-116">VisualElement</a>)</code></pre>
> Remove a child element.
> 
> **Parameters**:
> - `visualElement`: The visual element to remove.
> 
<pre class="language-typescript"><code class="lang-typescript">function RemoveFromHierarchy()</code></pre>
> Removes this element from its parent hierarchy.
> 
<pre class="language-typescript"><code class="lang-typescript">function Clear()</code></pre>
> Remove all child elements.
> 
<pre class="language-typescript"><code class="lang-typescript">function GetElementAt(index: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Get child element at index.
> 
> **Parameters**:
> - `index`: The index of the child element to get.
> 
<pre class="language-typescript"><code class="lang-typescript">function QueryByName(name: string) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Query child element by name.
> 
> **Parameters**:
> - `name`: The name of the element to find.
> 
> **Returns**: The first child element with the matching name.
<pre class="language-typescript"><code class="lang-typescript">function QueryByClassName(className: string) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Query child element by class name.
> 
> **Parameters**:
> - `className`: The class name of the element to find.
> 
> **Returns**: The first child element with the matching class name.
<pre class="language-typescript"><code class="lang-typescript">function RegisterMouseEnterEventCallback(method: function) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Register a callback for mouse enter event. Mouse enter event is fired when the mouse pointer enters an element or one of its children.
> 
> **Parameters**:
> - `method`: The method to call when the mouse enters the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function RegisterMouseLeaveEventCallback(method: function) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Register a callback for mouse leave event. Mouse leave event is fired when the mouse pointer exits an element and all its children.
> 
> **Parameters**:
> - `method`: The method to call when the mouse leaves the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function RegisterClickEventCallback(method: function) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Register a callback for click event.
> 
> **Parameters**:
> - `method`: The method to call when the element is clicked.
> 
<pre class="language-typescript"><code class="lang-typescript">function RegisterFocusInEventCallback(method: function) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Register a callback for focus in event. Focus in event is fired immediately before an element gains focus.
> 
> **Parameters**:
> - `method`: The method to call when the element gains focus.
> 
<pre class="language-typescript"><code class="lang-typescript">function RegisterFocusOutEventCallback(method: function) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Register a callback for focus out event. Focus out event is fired immediately before an element loses focus.
> 
> **Parameters**:
> - `method`: The method to call when the element loses focus.
> 
<pre class="language-typescript"><code class="lang-typescript">function Opacity(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the opacity of the element.
> 
> **Parameters**:
> - `value`: A value between 0 and 100.
> 
<pre class="language-typescript"><code class="lang-typescript">function Active(value: bool = True) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the element to be active or inactive.
> 
<pre class="language-typescript"><code class="lang-typescript">function Visible(value: bool = True) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the element to be visible or hidden.
> 
<pre class="language-typescript"><code class="lang-typescript">function TransitionDuration(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the transition duration of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function Absolute(value: bool = True) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the element to be absolute or relative positioned.
> 
<pre class="language-typescript"><code class="lang-typescript">function Left(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the left position of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function Top(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the top position of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function Right(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the right position of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function Bottom(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the bottom position of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function FlexShrink(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the flex shrink value.
> 
<pre class="language-typescript"><code class="lang-typescript">function FlexGrow(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the flex grow value.
> 
<pre class="language-typescript"><code class="lang-typescript">function FlexDirection(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the flex direction.
> 
> **Parameters**:
> - `value`: Acceptable values are: `Row`, `Column`, `RowReverse`, and `ColumnReverse`. Refer to [FlexDirectionEnum](../Enums/FlexDirectionEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function FlexWrap(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the wrap property.
> 
> **Parameters**:
> - `value`: Acceptable values are: `NoWrap`, `Wrap`, `WrapReverse`. Refer to [WrapEnum](../Enums/WrapEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function AlignItems(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the align items property.
> 
> **Parameters**:
> - `value`: Acceptable values are: `Auto`, `FlexStart`, `Center`, `FlexEnd`, and `Stretch`. Refer to [AlignEnum](../Enums/AlignEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function JustifyContent(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the justify content property.
> 
> **Parameters**:
> - `value`: Acceptable values are: `FlexStart`, `Center`, `FlexEnd`, `SpaceBetween`, `SpaceAround`, and `SpaceEvenly`. Refer to [JustifyEnum](../Enums/JustifyEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function AlignSelf(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the align self property.
> 
> **Parameters**:
> - `value`: Acceptable values are: `Auto`, `FlexStart`, `Center`, `FlexEnd`, and `Stretch`. Refer to [AlignEnum](../Enums/AlignEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function Width(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the width of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function Height(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the height of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function MinWidth(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the minimum width of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function MinHeight(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the minimum height of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function MaxWidth(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the maximum width of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function MaxHeight(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the maximum height of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function AspectRatio(value: float, mode: int = 0) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the height of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `mode`: Determines the direction of the aspect ratio. Acceptable values are: `Width` and `Height` Refer to [AspectRatioEnum](../Enums/AspectRatioEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function Margin(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the margin of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function MarginLeft(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the left margin of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function MarginTop(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the top margin of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function MarginRight(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the right margin of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function MarginBottom(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the bottom margin of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function Padding(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the padding of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function PaddingLeft(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the left padding of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function PaddingTop(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the top padding of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function PaddingRight(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the right padding of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function PaddingBottom(value: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the bottom padding of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function FontStyle(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the font style of the element.
> 
> **Parameters**:
> - `value`: Acceptable values are: `Normal`, `Bold`, `Italic`, and `BoldAndItalic`. Refer to [FontStyleEnum](../Enums/FontStyleEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function FontSize(value: float, percentage: bool = False, scaleMode: int = 0) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the font size of the element.
> 
> **Parameters**:
> - `value`: The value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> - `scaleMode`: Determines the container dimension used for percentage calculations. Acceptable values are: `Width`, `Height`. Refer to [FontScaleModeEnum](../Enums/FontScaleModeEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function Color(color: <a data-footnote-ref href="#user-content-fn-0">Color</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text color of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextAlign(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text alignment of the element.
> 
> **Parameters**:
> - `value`: Valid values are: `UpperLeft`, `UpperCenter`, `UpperRight`, `MiddleLeft`, `MiddleCenter`, `MiddleRight`, `LowerLeft`, `LowerCenter`, `LowerRight`. Refer to [TextAlignEnum](../Enums/TextAlignEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function TextWrap(value: bool = True) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set whether the text should wrap or not.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextOverflow(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text overflow behavior.
> 
> **Parameters**:
> - `value`: Acceptable values are: `Clip`, `Ellipsis`. Refer to [TextOverflowEnum](../Enums/TextOverflowEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function TextOutlineWidth(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text outline width.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextOutlineColor(value: <a data-footnote-ref href="#user-content-fn-0">Color</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text outline color.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextShadowColor(value: <a data-footnote-ref href="#user-content-fn-0">Color</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text shadow color.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextShadowOffset(horizontal: float, vertical: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text shadow offset.
> 
> **Parameters**:
> - `horizontal`: Horizontal offset.
> - `vertical`: Vertical offset.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextShadowHorizontalOffset(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text shadow horizontal offset.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextShadowVerticalOffset(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text shadow vertical offset.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextShadowBlurRadius(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text shadow blur radius.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextLetterSpacing(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text letter spacing.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextWordSpacing(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text word spacing.
> 
<pre class="language-typescript"><code class="lang-typescript">function TextParagraphSpacing(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the text paragraph spacing.
> 
<pre class="language-typescript"><code class="lang-typescript">function BackgroundColor(color: <a data-footnote-ref href="#user-content-fn-0">Color</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the background color of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function SetBackgroundImage(image: <a data-footnote-ref href="#user-content-fn-108">Image</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the background image of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderColor(color: <a data-footnote-ref href="#user-content-fn-0">Color</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the border color of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderColorLeft(color: <a data-footnote-ref href="#user-content-fn-0">Color</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the left border color of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderColorTop(color: <a data-footnote-ref href="#user-content-fn-0">Color</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the top border color of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderColorRight(color: <a data-footnote-ref href="#user-content-fn-0">Color</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the right border color of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderColorBottom(color: <a data-footnote-ref href="#user-content-fn-0">Color</a>) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the bottom border color of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderWidth(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the border width of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderWidthLeft(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the left border width of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderWidthTop(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the top border width of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderWidthRight(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the right border width of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderWidthBottom(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the bottom border width of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderRadius(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the border radius of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderRadiusTopLeft(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the top-left border radius of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderRadiusTopRight(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the top-right border radius of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderRadiusBottomLeft(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the bottom-left border radius of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function BorderRadiusBottomRight(value: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the bottom-right border radius of the element.
> 
<pre class="language-typescript"><code class="lang-typescript">function OverflowX(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the overflow behavior on the X axis.
> 
> **Parameters**:
> - `value`: Acceptable values are: `Visible` and `Hidden`. Refer to [OverflowEnum](../Enums/OverflowEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function OverflowY(value: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the overflow behavior on the Y axis.
> 
> **Parameters**:
> - `value`: Acceptable values are: `Visible` and `Hidden`. Refer to [OverflowEnum](../Enums/OverflowEnum.md)
> 
<pre class="language-typescript"><code class="lang-typescript">function SetTransformOrigin(x: float, y: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Set the origin of the element.
> 
> **Parameters**:
> - `x`: X value.
> - `y`: Y value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function TransformTranslate(x: float, y: float, percentage: bool = False) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Translate the element.
> 
> **Parameters**:
> - `x`: X value.
> - `y`: Y value.
> - `percentage`: If true, the `value` will be treated as percentage value.
> 
<pre class="language-typescript"><code class="lang-typescript">function TransformScale(x: float, y: float) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Scale the element.
> 
> **Parameters**:
> - `x`: X value.
> - `y`: Y value.
> 
<pre class="language-typescript"><code class="lang-typescript">function TransformRotate(angle: float, angleUnit: int) -> <a data-footnote-ref href="#user-content-fn-116">VisualElement</a></code></pre>
> Rotate the element.
> 
> **Parameters**:
> - `angle`: The angle of rotation.
> - `angleUnit`: The unit of the angle. Valid values are: `Degree`, `Gradian`, `Radian`, and `Turn`. Refer to [AngleUnitEnum](../Enums/AngleUnitEnum.md)
> 

[^0]: [Color](../Collections/Color.md)
[^1]: [Dict](../Collections/Dict.md)
[^2]: [LineCastHitResult](../Collections/LineCastHitResult.md)
[^3]: [List](../Collections/List.md)
[^4]: [Quaternion](../Collections/Quaternion.md)
[^5]: [Range](../Collections/Range.md)
[^6]: [Set](../Collections/Set.md)
[^7]: [Vector2](../Collections/Vector2.md)
[^8]: [Vector3](../Collections/Vector3.md)
[^9]: [Animation](../Component/Animation.md)
[^10]: [Animator](../Component/Animator.md)
[^11]: [AudioSource](../Component/AudioSource.md)
[^12]: [Collider](../Component/Collider.md)
[^13]: [Collision](../Component/Collision.md)
[^14]: [LightBuiltin](../Component/LightBuiltin.md)
[^15]: [LineRenderer](../Component/LineRenderer.md)
[^16]: [LodBuiltin](../Component/LodBuiltin.md)
[^17]: [MapTargetable](../Component/MapTargetable.md)
[^18]: [NavmeshObstacleBuiltin](../Component/NavmeshObstacleBuiltin.md)
[^19]: [PhysicsMaterialBuiltin](../Component/PhysicsMaterialBuiltin.md)
[^20]: [RigidbodyBuiltin](../Component/RigidbodyBuiltin.md)
[^21]: [VideoPlayer](../Component/VideoPlayer.md)
[^22]: [Character](../Entities/Character.md)
[^23]: [Human](../Entities/Human.md)
[^24]: [MapObject](../Entities/MapObject.md)
[^25]: [NetworkView](../Entities/NetworkView.md)
[^26]: [Player](../Entities/Player.md)
[^27]: [Prefab](../Entities/Prefab.md)
[^28]: [Shifter](../Entities/Shifter.md)
[^29]: [Titan](../Entities/Titan.md)
[^30]: [Transform](../Entities/Transform.md)
[^31]: [WallColossal](../Entities/WallColossal.md)
[^32]: [AlignEnum](../Enums/AlignEnum.md)
[^33]: [AngleUnitEnum](../Enums/AngleUnitEnum.md)
[^34]: [AnnieAnimationEnum](../Enums/AnnieAnimationEnum.md)
[^35]: [AspectRatioEnum](../Enums/AspectRatioEnum.md)
[^36]: [CameraModeEnum](../Enums/CameraModeEnum.md)
[^37]: [CharacterTypeEnum](../Enums/CharacterTypeEnum.md)
[^38]: [CollideModeEnum](../Enums/CollideModeEnum.md)
[^39]: [CollideWithEnum](../Enums/CollideWithEnum.md)
[^40]: [CollisionDetectionModeEnum](../Enums/CollisionDetectionModeEnum.md)
[^41]: [DummyAnimationEnum](../Enums/DummyAnimationEnum.md)
[^42]: [EffectNameEnum](../Enums/EffectNameEnum.md)
[^43]: [ErenAnimationEnum](../Enums/ErenAnimationEnum.md)
[^44]: [FlexDirectionEnum](../Enums/FlexDirectionEnum.md)
[^45]: [FontScaleModeEnum](../Enums/FontScaleModeEnum.md)
[^46]: [FontStyleEnum](../Enums/FontStyleEnum.md)
[^47]: [ForceModeEnum](../Enums/ForceModeEnum.md)
[^48]: [GradientModeEnum](../Enums/GradientModeEnum.md)
[^49]: [HandStateEnum](../Enums/HandStateEnum.md)
[^50]: [HorseAnimationEnum](../Enums/HorseAnimationEnum.md)
[^51]: [HumanAnimationEnum](../Enums/HumanAnimationEnum.md)
[^52]: [HumanParticleEffectEnum](../Enums/HumanParticleEffectEnum.md)
[^53]: [HumanSoundEnum](../Enums/HumanSoundEnum.md)
[^54]: [HumanStateEnum](../Enums/HumanStateEnum.md)
[^55]: [InputAnnieShifterEnum](../Enums/InputAnnieShifterEnum.md)
[^56]: [InputCategoryEnum](../Enums/InputCategoryEnum.md)
[^57]: [InputErenShifterEnum](../Enums/InputErenShifterEnum.md)
[^58]: [InputGeneralEnum](../Enums/InputGeneralEnum.md)
[^59]: [InputHumanEnum](../Enums/InputHumanEnum.md)
[^60]: [InputInteractionEnum](../Enums/InputInteractionEnum.md)
[^61]: [InputTitanEnum](../Enums/InputTitanEnum.md)
[^62]: [JustifyEnum](../Enums/JustifyEnum.md)
[^63]: [LanguageEnum](../Enums/LanguageEnum.md)
[^64]: [LineAlignmentEnum](../Enums/LineAlignmentEnum.md)
[^65]: [LineTextureModeEnum](../Enums/LineTextureModeEnum.md)
[^66]: [LoadoutEnum](../Enums/LoadoutEnum.md)
[^67]: [OutlineModeEnum](../Enums/OutlineModeEnum.md)
[^68]: [OverflowEnum](../Enums/OverflowEnum.md)
[^69]: [PhysicMaterialCombineEnum](../Enums/PhysicMaterialCombineEnum.md)
[^70]: [PlayerStatusEnum](../Enums/PlayerStatusEnum.md)
[^71]: [ProfileIconEnum](../Enums/ProfileIconEnum.md)
[^72]: [ProjectileNameEnum](../Enums/ProjectileNameEnum.md)
[^73]: [ScaleModeEnum](../Enums/ScaleModeEnum.md)
[^74]: [ScrollElasticityEnum](../Enums/ScrollElasticityEnum.md)
[^75]: [ShadowCastingModeEnum](../Enums/ShadowCastingModeEnum.md)
[^76]: [ShifterSoundEnum](../Enums/ShifterSoundEnum.md)
[^77]: [ShifterTypeEnum](../Enums/ShifterTypeEnum.md)
[^78]: [SliderDirectionEnum](../Enums/SliderDirectionEnum.md)
[^79]: [SpecialEnum](../Enums/SpecialEnum.md)
[^80]: [SteamStateEnum](../Enums/SteamStateEnum.md)
[^81]: [StunStateEnum](../Enums/StunStateEnum.md)
[^82]: [TeamEnum](../Enums/TeamEnum.md)
[^83]: [TextAlignEnum](../Enums/TextAlignEnum.md)
[^84]: [TextOverflowEnum](../Enums/TextOverflowEnum.md)
[^85]: [TitanAnimationEnum](../Enums/TitanAnimationEnum.md)
[^86]: [TitanSoundEnum](../Enums/TitanSoundEnum.md)
[^87]: [TitanTypeEnum](../Enums/TitanTypeEnum.md)
[^88]: [TSKillSoundEnum](../Enums/TSKillSoundEnum.md)
[^89]: [UILabelEnum](../Enums/UILabelEnum.md)
[^90]: [UnityComponentEnum](../Enums/UnityComponentEnum.md)
[^91]: [WallColossalAnimationEnum](../Enums/WallColossalAnimationEnum.md)
[^92]: [WeaponEnum](../Enums/WeaponEnum.md)
[^93]: [WrapEnum](../Enums/WrapEnum.md)
[^94]: [Camera](../Game/Camera.md)
[^95]: [Cutscene](../Game/Cutscene.md)
[^96]: [Game](../Game/Game.md)
[^97]: [Input](../Game/Input.md)
[^98]: [Locale](../Game/Locale.md)
[^99]: [Map](../Game/Map.md)
[^100]: [Network](../Game/Network.md)
[^101]: [PersistentData](../Game/PersistentData.md)
[^102]: [Physics](../Game/Physics.md)
[^103]: [RoomData](../Game/RoomData.md)
[^104]: [Time](../Game/Time.md)
[^105]: [Button](../UIElements/Button.md)
[^106]: [Dropdown](../UIElements/Dropdown.md)
[^107]: [Icon](../UIElements/Icon.md)
[^108]: [Image](../UIElements/Image.md)
[^109]: [Label](../UIElements/Label.md)
[^110]: [ProgressBar](../UIElements/ProgressBar.md)
[^111]: [ScrollView](../UIElements/ScrollView.md)
[^112]: [Slider](../UIElements/Slider.md)
[^113]: [TextField](../UIElements/TextField.md)
[^114]: [Toggle](../UIElements/Toggle.md)
[^115]: [UI](../UIElements/UI.md)
[^116]: [VisualElement](../UIElements/VisualElement.md)
[^117]: [Convert](../Utility/Convert.md)
[^118]: [Json](../Utility/Json.md)
[^119]: [Math](../Utility/Math.md)
[^120]: [Random](../Utility/Random.md)
[^121]: [String](../Utility/String.md)
[^122]: [Object](../objects/Object.md)
[^123]: [Component](../objects/Component.md)
