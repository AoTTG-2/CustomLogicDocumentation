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
#### <mark style="color:#509cd4;">[Transform](../objects/Transform.md)</mark> <mark style="color:#dcdcaa;">GetTransform</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">name</mark>)
Gets the transform of the specified child.
#### <mark style="color:#509cd4;">[List](../objects/List.md)</mark> <mark style="color:#dcdcaa;">GetTransforms</mark>()
Gets all child transforms.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">PlayAnimation</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">anim</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">fade</mark> = <mark style="color:#509cd4;">0.1</mark>)
Plays the specified animation.
#### <mark style="color:#509cd4;">float</mark> <mark style="color:#dcdcaa;">GetAnimationLength</mark>(<mark style="color:#509cd4;">[String](../static/String.md)</mark> <mark style="color:#9cdcfe;">anim</mark>)
Gets the length of the specified animation.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">PlaySound</mark>()
Plays the sound.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">StopSound</mark>()
Stops the sound.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">ToggleParticle</mark>(<mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">enabled</mark>)
Toggles the particle system.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">InverseTransformDirection</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">direction</mark>)
Transforms a direction from world space to local space. The opposite of Transform.TransformDirection.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">InverseTransformPoint</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">point</mark>)
Transforms position from world space to local space.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">TransformDirection</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">direction</mark>)
Transforms direction from local space to world space.
#### <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#dcdcaa;">TransformPoint</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">point</mark>)
Transforms position from local space to world space.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">Rotate</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">rotation</mark>)
Applies a rotation of eulerAngles.z degrees around the z-axis, eulerAngles.x degrees around the x-axis, and eulerAngles.y degrees around the y-axis (in that order).
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">RotateAround</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">point</mark>, <mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">axis</mark>, <mark style="color:#509cd4;">float</mark> <mark style="color:#9cdcfe;">angle</mark>)
Rotates the transform about axis passing through point in world coordinates by angle degrees.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">LookAt</mark>(<mark style="color:#509cd4;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:#9cdcfe;">target</mark>)
Rotates the transform so the forward vector points at worldPosition.
#### <mark style="color:#509cd4;">void</mark> <mark style="color:#dcdcaa;">SetRenderersEnabled</mark>(<mark style="color:#509cd4;">bool</mark> <mark style="color:#9cdcfe;">enabled</mark>)
Sets the enabled state of all child renderers.

---

