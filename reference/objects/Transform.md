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
#### <mark style="color:Blue;">[Transform](../objects/Transform.md)</mark> <mark style="color:Yellow;">GetTransform</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">name</mark>)
Gets the transform of the specified child.
#### <mark style="color:Blue;">[List](../objects/List.md)</mark> <mark style="color:Yellow;">GetTransforms</mark>()
Gets all child transforms.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">PlayAnimation</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">anim</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">fade</mark> = <mark style="color:Blue;">0.1</mark>)
Plays the specified animation.
#### <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">GetAnimationLength</mark>(<mark style="color:Blue;">[String](../static/String.md)</mark> <mark style="color:Yellow;">anim</mark>)
Gets the length of the specified animation.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">PlaySound</mark>()
Plays the sound.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">StopSound</mark>()
Stops the sound.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">ToggleParticle</mark>(<mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">enabled</mark>)
Toggles the particle system.
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">InverseTransformDirection</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">direction</mark>)
Transforms a direction from world space to local space. The opposite of Transform.TransformDirection.
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">InverseTransformPoint</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">point</mark>)
Transforms position from world space to local space.
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">TransformDirection</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">direction</mark>)
Transforms direction from local space to world space.
#### <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">TransformPoint</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">point</mark>)
Transforms position from local space to world space.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">Rotate</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">rotation</mark>)
Applies a rotation of eulerAngles.z degrees around the z-axis, eulerAngles.x degrees around the x-axis, and eulerAngles.y degrees around the y-axis (in that order).
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">RotateAround</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">point</mark>, <mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">axis</mark>, <mark style="color:Blue;">float</mark> <mark style="color:Yellow;">angle</mark>)
Rotates the transform about axis passing through point in world coordinates by angle degrees.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">LookAt</mark>(<mark style="color:Blue;">[Vector3](../objects/Vector3.md)</mark> <mark style="color:Yellow;">target</mark>)
Rotates the transform so the forward vector points at worldPosition.
#### <mark style="color:Blue;">void</mark> <mark style="color:Yellow;">SetRenderersEnabled</mark>(<mark style="color:Blue;">bool</mark> <mark style="color:Yellow;">enabled</mark>)
Sets the enabled state of all child renderers.

---

