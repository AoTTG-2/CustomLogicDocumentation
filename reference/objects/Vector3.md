# Vector3
Inherits from [Object](./Object.md)
### Remarks
Overloads operators: 
- `__Copy__`
- `+`
- `-`
- `*`
- `/`
- `==`
- `__Hash__`
### Initialization
```csharp
Vector3() # Default constructor. Initializes the Vector3 to (0, 0, 0).
Vector3(xyz: float) # Default constructor. Initializes the Vector3 to (xyz, xyz, xyz).
Vector3(x: float, y: float)
Vector3(x: float, y: float, z: float)
```

### Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|X|float|False|X component of the vector.|
|Y|float|False|Y component of the vector.|
|Z|float|False|Z component of the vector.|
|Normalized|[Vector3](./Vector3.md)|True|Returns this vector with a magnitude of 1 (Read Only).|
|Magnitude|float|True|Returns the length of this vector (Read Only).|
|SqrMagnitude|float|True|Returns the squared length of this vector (Read Only).|


### Static Properties
|Name|Type|Readonly|Description|
|---|---|---|---|
|Zero|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(0, 0, 0).|
|One|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(1, 1, 1).|
|Up|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(0, 1, 0).|
|Down|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(0, -1, 0).|
|Left|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(-1, 0, 0).|
|Right|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(1, 0, 0).|
|Forward|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(0, 0, 1).|
|Back|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(0, 0, -1).|
|NegativeInfinity|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(float.PositiveInfinity, float.PositiveInfinity, float.PositiveInfinity).|
|PositiveInfinity|[Vector3](./Vector3.md)|True|Shorthand for writing Vector3(float.PositiveInfinity, float.PositiveInfinity, float.PositiveInfinity).|


### Methods
<pre class="language-typescript"><code class="lang-typescript">function Set(x: float, y: float, z: float) -> null</code></pre>
> Set x, y and z components of an existing Vector3.

<pre class="language-typescript"><code class="lang-typescript">function Scale(scale: <a data-footnote-ref href="#user-content-fn-37">Object</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>

%{ hint style="warning" %}
**Obsolete**: Use multiply operator instead
%{ endhint %}
> Returns the Vector3 multiplied by scale.

> **Parameters**:
> - `scale`: float | Vector3

<pre class="language-typescript"><code class="lang-typescript">function Multiply(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>

%{ hint style="warning" %}
**Obsolete**: Use multiply operator instead
%{ endhint %}
> Returns the multiplication of two Vector3s.

> **Parameters**:
> - `a`: Vector3
> - `b`: Vector3

> **Returns**: Vector3
<pre class="language-typescript"><code class="lang-typescript">function Divide(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>

%{ hint style="warning" %}
**Obsolete**: Use divide operator instead
%{ endhint %}
> Returns the division of two Vector3s.

> **Parameters**:
> - `a`: Vector3
> - `b`: Vector3

> **Returns**: Vector3
<pre class="language-typescript"><code class="lang-typescript">function GetRotationDirection(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Gets the relational Vector3 "b" using "a" as a reference. This is equivalent to setting MapObject.Forward to Vector "a", and finding the relative "b" vector.


### Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Angle(from: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, to: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> float</code></pre>
> Calculates the angle between vectors from and.

> **Returns**: The angle in degrees between the two vectors.
<pre class="language-typescript"><code class="lang-typescript">function ClampMagnitude(vector: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, maxLength: float) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Returns a copy of vector with its magnitude clamped to maxLength.

<pre class="language-typescript"><code class="lang-typescript">function Cross(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Cross Product of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Distance(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> float</code></pre>
> Returns the distance between a and b.

<pre class="language-typescript"><code class="lang-typescript">function Dot(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> float</code></pre>
> Dot Product of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Lerp(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Linearly interpolates between two points.

> **Returns**: Interpolated value, equals to a + (b - a) * t.
<pre class="language-typescript"><code class="lang-typescript">function LerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Linearly interpolates between two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Max(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Returns a vector that is made from the largest components of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Min(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Returns a vector that is made from the smallest components of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function MoveTowards(current: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, target: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, maxDistanceDelta: float) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Calculate a position between the points specified by current and target, moving no farther than the distance specified by maxDistanceDelta.

> **Returns**: The new position.
<pre class="language-typescript"><code class="lang-typescript">function Normalize(value: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Makes this vector have a magnitude of 1.

<pre class="language-typescript"><code class="lang-typescript">function OrthoNormalize(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> null</code></pre>
<pre class="language-typescript"><code class="lang-typescript">function Project(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Projects a vector onto another vector.

<pre class="language-typescript"><code class="lang-typescript">function ProjectOnPlane(vector: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, plane: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Projects a vector onto a plane defined by a normal orthogonal to the plane.

> **Returns**: The location of the vector on the plane.
<pre class="language-typescript"><code class="lang-typescript">function Reflect(inDirection: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, inNormal: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Reflects a vector off the plane defined by a normal.

<pre class="language-typescript"><code class="lang-typescript">function RotateTowards(current: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, target: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, maxRadiansDelta: float, maxMagnitudeDelta: float) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Rotates a vector current towards target.

> **Returns**: The location that RotateTowards generates.
<pre class="language-typescript"><code class="lang-typescript">function SignedAngle(from: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, to: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, axis: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>) -> float</code></pre>
> Calculates the signed angle between vectors from and to in relation to axis.

> **Returns**: Returns the signed angle between from and to in degrees.
<pre class="language-typescript"><code class="lang-typescript">function Slerp(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Spherically interpolates between two vectors.

<pre class="language-typescript"><code class="lang-typescript">function SlerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, t: float) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>
> Spherically interpolates between two vectors.

<pre class="language-typescript"><code class="lang-typescript">function SmoothDamp(current: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, target: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, currentVelocity: <a data-footnote-ref href="#user-content-fn-36">Vector3</a>, smoothTime: float, maxSpeed: float) -> <a data-footnote-ref href="#user-content-fn-36">Vector3</a></code></pre>

[^1]: [Camera](./Camera.md)
[^2]: [Character](./Character.md)
[^3]: [Collider](./Collider.md)
[^4]: [Collision](./Collision.md)
[^5]: [Color](./Color.md)
[^6]: [Convert](./Convert.md)
[^7]: [Cutscene](./Cutscene.md)
[^8]: [Dict](./Dict.md)
[^9]: [Game](./Game.md)
[^10]: [Human](./Human.md)
[^11]: [Input](./Input.md)
[^12]: [Json](./Json.md)
[^13]: [LineCastHitResult](./LineCastHitResult.md)
[^14]: [LineRenderer](./LineRenderer.md)
[^15]: [List](./List.md)
[^16]: [Map](./Map.md)
[^17]: [MapObject](./MapObject.md)
[^18]: [MapTargetable](./MapTargetable.md)
[^19]: [Math](./Math.md)
[^20]: [Network](./Network.md)
[^21]: [NetworkView](./NetworkView.md)
[^22]: [PersistentData](./PersistentData.md)
[^23]: [Physics](./Physics.md)
[^24]: [Player](./Player.md)
[^25]: [Quaternion](./Quaternion.md)
[^26]: [Random](./Random.md)
[^27]: [Range](./Range.md)
[^28]: [RoomData](./RoomData.md)
[^29]: [Set](./Set.md)
[^30]: [Shifter](./Shifter.md)
[^31]: [String](./String.md)
[^32]: [Time](./Time.md)
[^33]: [Titan](./Titan.md)
[^34]: [Transform](./Transform.md)
[^35]: [UI](./UI.md)
[^36]: [Vector2](./Vector2.md)
[^37]: [Vector3](./Vector3.md)
[^38]: [Object](./Object.md)
