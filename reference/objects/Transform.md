# Transform
Inherits from object
## Initialization
```csharp
```
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Position|[Vector3](../objects/Vector3.md)|False|Gets or sets the position of the transform.|
|LocalPosition|[Vector3](../objects/Vector3.md)|False|Gets or sets the local position of the transform.|
|Rotation|[Vector3](../objects/Vector3.md)|False|Gets or sets the rotation of the transform.|
|LocalRotation|[Vector3](../objects/Vector3.md)|False|Gets or sets the local rotation of the transform.|
|QuaternionRotation|[Quaternion](../objects/Quaternion.md)|False|Gets or sets the quaternion rotation of the transform.|
|QuaternionLocalRotation|[Quaternion](../objects/Quaternion.md)|False|Gets or sets the quaternion local rotation of the transform.|
|Scale|[Vector3](../objects/Vector3.md)|False|Gets or sets the scale of the transform.|
|Forward|[Vector3](../objects/Vector3.md)|False|Gets the forward vector of the transform.|
|Up|[Vector3](../objects/Vector3.md)|False|Gets the up vector of the transform.|
|Right|[Vector3](../objects/Vector3.md)|False|Gets the right vector of the transform.|
## Methods
#### <mark style="color:blue;">[Transform](../objects/Transform.md)</mark> <mark style="color:yellow;">GetTransform</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> name)
> Gets the transform of the specified child.

#### <mark style="color:blue;">[List](../objects/List.md)</mark> <mark style="color:yellow;">GetTransforms</mark>()
> Gets all child transforms.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">PlayAnimation</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> anim, <mark style="color:blue;">float</mark> fade = <mark style="color:blue;">0.1</mark>)
> Plays the specified animation.

#### <mark style="color:blue;">float</mark> <mark style="color:yellow;">GetAnimationLength</mark>(<mark style="color:blue;">[String](../static/String.md)</mark> anim)
> Gets the length of the specified animation.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">PlaySound</mark>()
> Plays the sound.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">StopSound</mark>()
> Stops the sound.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">ToggleParticle</mark>(<mark style="color:blue;">bool</mark> enabled)
> Toggles the particle system.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">InverseTransformDirection</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> direction)
> Transforms a direction from world space to local space. The opposite of Transform.TransformDirection.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">InverseTransformPoint</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> point)
> Transforms position from world space to local space.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">TransformDirection</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> direction)
> Transforms direction from local space to world space.

#### <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:yellow;">TransformPoint</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> point)
> Transforms position from local space to world space.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">Rotate</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> rotation)
> Applies a rotation of eulerAngles.z degrees around the z-axis, eulerAngles.x degrees around the x-axis, and eulerAngles.y degrees around the y-axis (in that order).

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">RotateAround</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> point, <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> axis, <mark style="color:blue;">float</mark> angle)
> Rotates the transform about axis passing through point in world coordinates by angle degrees.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">LookAt</mark>(<mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark> target)
> Rotates the transform so the forward vector points at worldPosition.

#### <mark style="color:blue;">void</mark> <mark style="color:yellow;">SetRenderersEnabled</mark>(<mark style="color:blue;">bool</mark> enabled)
> Sets the enabled state of all child renderers.


---

