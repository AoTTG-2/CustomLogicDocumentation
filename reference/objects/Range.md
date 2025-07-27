# Range

Inherits from List. Allows you to create lists of integers for convenient iteration, particularly in for loops.

### Example
```csharp
for (a in Range(10))
Game.Print(a);

for (a in Range(1, 10))
Game.Print(a);

for (a in Range(1, 10, 2))
Game.Print(a);
```
### Initialization
```csharp
Range(parameterValues: Object) # The constructor for the Range builtin class has multiple overloads.
Range(n) creates a range from 0 to n-1.
Range(a, n) creates a range from a to n-1.
Range(a, n, step) creates a range from a to n-1 with the specified step.
```

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Count|int|True|The number of elements in the list|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Clear() -> null</code></pre>
> Clear all list elements

<pre class="language-typescript"><code class="lang-typescript">function Get(index: int) -> <a data-footnote-ref href="#user-content-fn-Object">Object</a></code></pre>
> Get the element at the specified index

<pre class="language-typescript"><code class="lang-typescript">function Set(index: int, value: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Set the element at the specified index

<pre class="language-typescript"><code class="lang-typescript">function Add(value: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Add an element to the end of the list

<pre class="language-typescript"><code class="lang-typescript">function InsertAt(index: int, value: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Insert an element at the specified index

<pre class="language-typescript"><code class="lang-typescript">function RemoveAt(index: int) -> null</code></pre>
> Remove the element at the specified index

<pre class="language-typescript"><code class="lang-typescript">function Remove(value: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> null</code></pre>
> Remove the first occurrence of the specified element

<pre class="language-typescript"><code class="lang-typescript">function Contains(value: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> bool</code></pre>
> Check if the list contains the specified element

<pre class="language-typescript"><code class="lang-typescript">function Sort() -> null</code></pre>
> Sort the list

<pre class="language-typescript"><code class="lang-typescript">function SortCustom(method: function) -> null</code></pre>
> Sort the list using a custom method, expects a method with the signature int method(a,b)

<pre class="language-typescript"><code class="lang-typescript">function Filter(method: function) -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Filter the list using a custom method, expects a method with the signature bool method(element)

<pre class="language-typescript"><code class="lang-typescript">function Map(method: function) -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Map the list using a custom method, expects a method with the signature object method(element)

<pre class="language-typescript"><code class="lang-typescript">function Reduce(method: function, initialValue: <a data-footnote-ref href="#user-content-fn-Object">Object</a>) -> <a data-footnote-ref href="#user-content-fn-Object">Object</a></code></pre>
> Reduce the list using a custom method, expects a method with the signature object method(acc, element)

<pre class="language-typescript"><code class="lang-typescript">function Randomize() -> <a data-footnote-ref href="#user-content-fn-List">List</a></code></pre>
> Returns a randomized version of the list.

<pre class="language-typescript"><code class="lang-typescript">function ToSet() -> <a data-footnote-ref href="#user-content-fn-Set">Set</a></code></pre>
> Convert the list to a set


[^Camera]: [Camera](../md/static/Camera.md)
[^Character]: [Character](../md/objects/Character.md)
[^Collider]: [Collider](../md/objects/Collider.md)
[^Collision]: [Collision](../md/objects/Collision.md)
[^Color]: [Color](../md/objects/Color.md)
[^Convert]: [Convert](../md/static/Convert.md)
[^Cutscene]: [Cutscene](../md/static/Cutscene.md)
[^Dict]: [Dict](../md/objects/Dict.md)
[^Game]: [Game](../md/static/Game.md)
[^Human]: [Human](../md/objects/Human.md)
[^Input]: [Input](../md/static/Input.md)
[^Json]: [Json](../md/static/Json.md)
[^LineCastHitResult]: [LineCastHitResult](../md/objects/LineCastHitResult.md)
[^LineRenderer]: [LineRenderer](../md/objects/LineRenderer.md)
[^List]: [List](../md/objects/List.md)
[^Map]: [Map](../md/static/Map.md)
[^MapObject]: [MapObject](../md/objects/MapObject.md)
[^MapTargetable]: [MapTargetable](../md/objects/MapTargetable.md)
[^Math]: [Math](../md/static/Math.md)
[^Network]: [Network](../md/static/Network.md)
[^NetworkView]: [NetworkView](../md/objects/NetworkView.md)
[^PersistentData]: [PersistentData](../md/static/PersistentData.md)
[^Physics]: [Physics](../md/static/Physics.md)
[^Player]: [Player](../md/objects/Player.md)
[^Quaternion]: [Quaternion](../md/objects/Quaternion.md)
[^Random]: [Random](../md/objects/Random.md)
[^Range]: [Range](../md/objects/Range.md)
[^RoomData]: [RoomData](../md/static/RoomData.md)
[^Set]: [Set](../md/objects/Set.md)
[^Shifter]: [Shifter](../md/objects/Shifter.md)
[^String]: [String](../md/static/String.md)
[^Time]: [Time](../md/static/Time.md)
[^Titan]: [Titan](../md/objects/Titan.md)
[^Transform]: [Transform](../md/objects/Transform.md)
[^UI]: [UI](../md/static/UI.md)
[^Vector2]: [Vector2](../md/objects/Vector2.md)
[^Vector3]: [Vector3](../md/objects/Vector3.md)
[^Object]: [Object](../md/objects/Object.md)
[^Component]: [Component](../md/objects/Component.md)
