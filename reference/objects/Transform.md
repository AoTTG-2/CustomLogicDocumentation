# Transform
Inherits from object
## Initialization
<mark style="color:red;">No constructor given, object can only be accessed via builtins.</mark>## Fields
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
#### function <mark style="color:yellow;">GetTransform</mark>(name: <mark style="color:blue;">[String](../static/String.md)</mark>) -> <mark style="color:blue;">[Transform](../objects/Transform.md)</mark>
> Gets the transform of the specified child.

#### function <mark style="color:yellow;">GetTransforms</mark>() -> <mark style="color:blue;">[List](../objects/List.md)</mark>
> Gets all child transforms.

#### function <mark style="color:yellow;">PlayAnimation</mark>(anim: <mark style="color:blue;">[String](../static/String.md)</mark>, fade: <mark style="color:blue;">float</mark> = <mark style="color:blue;">0.1</mark>) -> <mark style="color:blue;">void</mark>
> Plays the specified animation.

#### function <mark style="color:yellow;">GetAnimationLength</mark>(anim: <mark style="color:blue;">[String](../static/String.md)</mark>) -> <mark style="color:blue;">float</mark>
> Gets the length of the specified animation.

#### function <mark style="color:yellow;">PlaySound</mark>() -> <mark style="color:blue;">void</mark>
> Plays the sound.

#### function <mark style="color:yellow;">StopSound</mark>() -> <mark style="color:blue;">void</mark>
> Stops the sound.

#### function <mark style="color:yellow;">ToggleParticle</mark>(enabled: <mark style="color:blue;">bool</mark>) -> <mark style="color:blue;">void</mark>
> Toggles the particle system.

#### function <mark style="color:yellow;">InverseTransformDirection</mark>(direction: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>) -> <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>
> Transforms a direction from world space to local space. The opposite of Transform.TransformDirection.

#### function <mark style="color:yellow;">InverseTransformPoint</mark>(point: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>) -> <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>
> Transforms position from world space to local space.

#### function <mark style="color:yellow;">TransformDirection</mark>(direction: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>) -> <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>
> Transforms direction from local space to world space.

#### function <mark style="color:yellow;">TransformPoint</mark>(point: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>) -> <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>
> Transforms position from local space to world space.

#### function <mark style="color:yellow;">Rotate</mark>(rotation: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>) -> <mark style="color:blue;">void</mark>
> Applies a rotation of eulerAngles.z degrees around the z-axis, eulerAngles.x degrees around the x-axis, and eulerAngles.y degrees around the y-axis (in that order).

#### function <mark style="color:yellow;">RotateAround</mark>(point: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>, axis: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>, angle: <mark style="color:blue;">float</mark>) -> <mark style="color:blue;">void</mark>
> Rotates the transform about axis passing through point in world coordinates by angle degrees.

#### function <mark style="color:yellow;">LookAt</mark>(target: <mark style="color:blue;">[Vector3](../objects/Vector3.md)</mark>) -> <mark style="color:blue;">void</mark>
> Rotates the transform so the forward vector points at worldPosition.

#### function <mark style="color:yellow;">SetRenderersEnabled</mark>(enabled: <mark style="color:blue;">bool</mark>) -> <mark style="color:blue;">void</mark>
> Sets the enabled state of all child renderers.


---

