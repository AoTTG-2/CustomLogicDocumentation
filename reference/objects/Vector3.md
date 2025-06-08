# Vector3
Inherits from Object

## Initialization
```csharp
# Vector3()
example = Vector3()

# Vector3(float)
example = Vector3(0)

# Vector3(float, float)
example = Vector3(0, 0)

# Vector3(float, float, float)
example = Vector3(0, 0, 0)
```
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|X|float|False|X component of the vector.|
|Y|float|False|Y component of the vector.|
|Z|float|False|Z component of the vector.|
|Normalized|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Returns this vector with a magnitude of 1 (Read Only).|
|Magnitude|float|True|Returns the length of this vector (Read Only).|
|SqrMagnitude|float|True|Returns the squared length of this vector (Read Only).|
## Static Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Zero|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(0, 0, 0).|
|One|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(1, 1, 1).|
|Up|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(0, 1, 0).|
|Down|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(0, -1, 0).|
|Left|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(-1, 0, 0).|
|Right|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(1, 0, 0).|
|Forward|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(0, 0, 1).|
|Back|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(0, 0, -1).|
|NegativeInfinity|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(float.PositiveInfinity, float.PositiveInfinity, float.PositiveInfinity).|
|PositiveInfinity|<a data-footnote-ref href="#user-content-fn-1">Vector3</a>|True|Shorthand for writing Vector3(float.PositiveInfinity, float.PositiveInfinity, float.PositiveInfinity).|
## Methods
<pre class="language-typescript"><code class="lang-typescript">function Set(x: float, y: float, z: float)</code></pre>
> Set x, y and z components of an existing Vector3.

<pre class="language-typescript"><code class="lang-typescript">function GetRotationDirection(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Gets the relational Vector3 "b" using "a" as a reference. This is equivalent to setting MapObject.Forward to Vector "a", and finding the relative "b" vector.

<pre class="language-typescript"><code class="lang-typescript">function __Copy__() → Object</code></pre>
> Overrides the assignment operator to create a deep copy of the object.

<pre class="language-typescript"><code class="lang-typescript">function __Add__(self: Object, other: Object) → Object</code></pre>
> Overrides addition, used for + operator. Ex: a + b is equivalent to a.\_\_Add\_\_(a, b)

<pre class="language-typescript"><code class="lang-typescript">function __Sub__(self: Object, other: Object) → Object</code></pre>
> Overrides subtraction, used for - operator. Ex: a - b is equivalent to a.\_\_Sub\_\_(a, b)

<pre class="language-typescript"><code class="lang-typescript">function __Mul__(self: Object, other: Object) → Object</code></pre>
> Overrides multiplication, used for * operator. Ex: a * b is equivalent to a.\_\_Mul\_\_(a, b)

<pre class="language-typescript"><code class="lang-typescript">function __Div__(self: Object, other: Object) → Object</code></pre>
> Overrides division, used for / operator. Ex: a / b is equivalent to a.\_\_Div\_\_(a, b)

<pre class="language-typescript"><code class="lang-typescript">function __Eq__(self: Object, other: Object) → bool</code></pre>
> Overrides the equality comparison, used for == and != operators. Ex: a == b is equivalent to a.\_\_Eq\_\_(a, b)

<pre class="language-typescript"><code class="lang-typescript">function __Hash__() → int</code></pre>
> Overrides hashing, used for GetHashCode - Used for Dictionaries/Sets. Ex: hash = obj.GetHashCode() is equivalent to hash = obj.\_\_Hash\_\_()

<pre class="language-typescript"><code class="lang-typescript">function Scale(scale: Object) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> <mark style="color:red;">This method is obselete</mark>: Use multiply operator instead

> Returns the Vector3 multiplied by scale.

<pre class="language-typescript"><code class="lang-typescript">function Multiply(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> <mark style="color:red;">This method is obselete</mark>: Use multiply operator instead

> Returns the multiplication of two Vector3s.

<pre class="language-typescript"><code class="lang-typescript">function Divide(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> <mark style="color:red;">This method is obselete</mark>: Use divide operator instead

> Returns the division of two Vector3s.


---

## Static Methods
<pre class="language-typescript"><code class="lang-typescript">function Angle(from: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, to: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → float</code></pre>
> Calculates the angle between vectors from and.

<pre class="language-typescript"><code class="lang-typescript">function ClampMagnitude(vector: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, maxLength: float) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Returns a copy of vector with its magnitude clamped to maxLength.

<pre class="language-typescript"><code class="lang-typescript">function Cross(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Cross Product of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Distance(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → float</code></pre>
> Returns the distance between a and b.

<pre class="language-typescript"><code class="lang-typescript">function Dot(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → float</code></pre>
> Dot Product of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Lerp(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, t: float) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Linearly interpolates between two points.

<pre class="language-typescript"><code class="lang-typescript">function LerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, t: float) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Linearly interpolates between two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Max(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Returns a vector that is made from the largest components of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function Min(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Returns a vector that is made from the smallest components of two vectors.

<pre class="language-typescript"><code class="lang-typescript">function MoveTowards(current: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, target: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, maxDistanceDelta: float) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Calculate a position between the points specified by current and target, moving no farther than the distance specified by maxDistanceDelta.

<pre class="language-typescript"><code class="lang-typescript">function Normalize(value: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Makes this vector have a magnitude of 1.

<pre class="language-typescript"><code class="lang-typescript">function OrthoNormalize(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>)</code></pre>
> <mark style="color:red;">Missing description, please ping dev to fix this or if you need clarification :)</mark>

<pre class="language-typescript"><code class="lang-typescript">function Project(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Projects a vector onto another vector.

<pre class="language-typescript"><code class="lang-typescript">function ProjectOnPlane(vector: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, plane: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Projects a vector onto a plane defined by a normal orthogonal to the plane.

<pre class="language-typescript"><code class="lang-typescript">function Reflect(inDirection: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, inNormal: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Reflects a vector off the plane defined by a normal.

<pre class="language-typescript"><code class="lang-typescript">function RotateTowards(current: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, target: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, maxRadiansDelta: float, maxMagnitudeDelta: float) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Rotates a vector current towards target.

<pre class="language-typescript"><code class="lang-typescript">function SignedAngle(from: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, to: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, axis: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>) → float</code></pre>
> Calculates the signed angle between vectors from and to in relation to axis.

<pre class="language-typescript"><code class="lang-typescript">function Slerp(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, t: float) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Spherically interpolates between two vectors.

<pre class="language-typescript"><code class="lang-typescript">function SlerpUnclamped(a: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, b: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, t: float) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> Spherically interpolates between two vectors.

<pre class="language-typescript"><code class="lang-typescript">function SmoothDamp(current: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, target: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, currentVelocity: <a data-footnote-ref href="#user-content-fn-1">Vector3</a>, smoothTime: float, maxSpeed: float) → <a data-footnote-ref href="#user-content-fn-1">Vector3</a></code></pre>
> <mark style="color:red;">Missing description, please ping dev to fix this or if you need clarification :)</mark>


---

[^1]: [Vector3](../objects/Vector3.md)