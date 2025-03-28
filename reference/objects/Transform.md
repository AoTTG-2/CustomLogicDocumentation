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
#### <span style="color:#509cd4;">[Transform](../objects/Transform.md)</span> <span style="color:#dcdcaa;">GetTransform</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">name</span>)
Gets the transform of the specified child.
#### <span style="color:#509cd4;">[List](../objects/List.md)</span> <span style="color:#dcdcaa;">GetTransforms</span>()
Gets all child transforms.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">PlayAnimation</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">anim</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">fade</span> = <span style="color:#509cd4;">0.1</span>)
Plays the specified animation.
#### <span style="color:#509cd4;">float</span> <span style="color:#dcdcaa;">GetAnimationLength</span>(<span style="color:#509cd4;">[String](../static/String.md)</span> <span style="color:#9cdcfe;">anim</span>)
Gets the length of the specified animation.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">PlaySound</span>()
Plays the sound.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">StopSound</span>()
Stops the sound.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">ToggleParticle</span>(<span style="color:#509cd4;">bool</span> <span style="color:#9cdcfe;">enabled</span>)
Toggles the particle system.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">InverseTransformDirection</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">direction</span>)
Transforms a direction from world space to local space. The opposite of Transform.TransformDirection.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">InverseTransformPoint</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">point</span>)
Transforms position from world space to local space.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">TransformDirection</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">direction</span>)
Transforms direction from local space to world space.
#### <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#dcdcaa;">TransformPoint</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">point</span>)
Transforms position from local space to world space.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">Rotate</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">rotation</span>)
Applies a rotation of eulerAngles.z degrees around the z-axis, eulerAngles.x degrees around the x-axis, and eulerAngles.y degrees around the y-axis (in that order).
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">RotateAround</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">point</span>, <span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">axis</span>, <span style="color:#509cd4;">float</span> <span style="color:#9cdcfe;">angle</span>)
Rotates the transform about axis passing through point in world coordinates by angle degrees.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">LookAt</span>(<span style="color:#509cd4;">[Vector3](../objects/Vector3.md)</span> <span style="color:#9cdcfe;">target</span>)
Rotates the transform so the forward vector points at worldPosition.
#### <span style="color:#509cd4;">void</span> <span style="color:#dcdcaa;">SetRenderersEnabled</span>(<span style="color:#509cd4;">bool</span> <span style="color:#9cdcfe;">enabled</span>)
Sets the enabled state of all child renderers.

---

