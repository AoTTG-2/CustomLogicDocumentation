# List
Inherits from [Object](../objects/Object.md)

List class for Custom Logic.

### Example
```csharp
values = List(1,2,1,4,115);

# Common generic list operations Map, Filter, Reduce, and Sort are supported.
# These methods take in a defined method with an expected signature and return type.

# Filter list to only unique values using set conversion.
uniques = values.ToSet().ToList();

# Accumulate values in list using reduce.
sum = values.Reduce(self.Sum2, 0);  # returns 123

# Filter list using predicate method.
filteredList = values.Filter(self.Filter);  # returns List(115)

# Transform list using mapping method.
newList = values.Map(self.TransformData);   # returns List(2,4,2,8,230)

function Sum2(a, b) {
return a + b;
}

function Filter(a) {
return a > 20;
}

function TransformData(a) {
return a * 2;
}
```
### Initialization
```csharp
List()
List(parameterValues: Object)
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


[^Camera]: [Camera](../static/Camera.md)
[^Character]: [Character](../objects/Character.md)
[^Collider]: [Collider](../objects/Collider.md)
[^Collision]: [Collision](../objects/Collision.md)
[^Color]: [Color](../objects/Color.md)
[^Convert]: [Convert](../static/Convert.md)
[^Cutscene]: [Cutscene](../static/Cutscene.md)
[^Dict]: [Dict](../objects/Dict.md)
[^Game]: [Game](../static/Game.md)
[^Human]: [Human](../objects/Human.md)
[^Input]: [Input](../static/Input.md)
[^Json]: [Json](../static/Json.md)
[^LineCastHitResult]: [LineCastHitResult](../objects/LineCastHitResult.md)
[^LineRenderer]: [LineRenderer](../objects/LineRenderer.md)
[^List]: [List](../objects/List.md)
[^Map]: [Map](../static/Map.md)
[^MapObject]: [MapObject](../objects/MapObject.md)
[^MapTargetable]: [MapTargetable](../objects/MapTargetable.md)
[^Math]: [Math](../static/Math.md)
[^Network]: [Network](../static/Network.md)
[^NetworkView]: [NetworkView](../objects/NetworkView.md)
[^PersistentData]: [PersistentData](../static/PersistentData.md)
[^Physics]: [Physics](../static/Physics.md)
[^Player]: [Player](../objects/Player.md)
[^Quaternion]: [Quaternion](../objects/Quaternion.md)
[^Random]: [Random](../objects/Random.md)
[^Range]: [Range](../objects/Range.md)
[^RoomData]: [RoomData](../static/RoomData.md)
[^Set]: [Set](../objects/Set.md)
[^Shifter]: [Shifter](../objects/Shifter.md)
[^String]: [String](../static/String.md)
[^Time]: [Time](../static/Time.md)
[^Titan]: [Titan](../objects/Titan.md)
[^Transform]: [Transform](../objects/Transform.md)
[^UI]: [UI](../static/UI.md)
[^Vector2]: [Vector2](../objects/Vector2.md)
[^Vector3]: [Vector3](../objects/Vector3.md)
[^Object]: [Object](../objects/Object.md)
[^Component]: [Component](../objects/Component.md)
