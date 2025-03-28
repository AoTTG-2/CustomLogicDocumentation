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
#### [Transform](../objects/Transform.md) <span style="color":#dcdcaa>GetTransform<span>([String](../static/String.md) <span style="color":#9cdcfe>name<span>)
Gets the transform of the specified child.
#### [List](../objects/List.md) <span style="color":#dcdcaa>GetTransforms<span>()
Gets all child transforms.
#### void <span style="color":#dcdcaa>PlayAnimation<span>([String](../static/String.md) <span style="color":#9cdcfe>anim<span>, float <span style="color":#9cdcfe>fade<span> = 0.1)
Plays the specified animation.
#### float <span style="color":#dcdcaa>GetAnimationLength<span>([String](../static/String.md) <span style="color":#9cdcfe>anim<span>)
Gets the length of the specified animation.
#### void <span style="color":#dcdcaa>PlaySound<span>()
Plays the sound.
#### void <span style="color":#dcdcaa>StopSound<span>()
Stops the sound.
#### void <span style="color":#dcdcaa>ToggleParticle<span>(bool <span style="color":#9cdcfe>enabled<span>)
Toggles the particle system.
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>InverseTransformDirection<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>direction<span>)
Transforms a direction from world space to local space. The opposite of Transform.TransformDirection.
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>InverseTransformPoint<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>point<span>)
Transforms position from world space to local space.
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>TransformDirection<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>direction<span>)
Transforms direction from local space to world space.
#### [Vector3](../objects/Vector3.md) <span style="color":#dcdcaa>TransformPoint<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>point<span>)
Transforms position from local space to world space.
#### void <span style="color":#dcdcaa>Rotate<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>rotation<span>)
Applies a rotation of eulerAngles.z degrees around the z-axis, eulerAngles.x degrees around the x-axis, and eulerAngles.y degrees around the y-axis (in that order).
#### void <span style="color":#dcdcaa>RotateAround<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>point<span>, [Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>axis<span>, float <span style="color":#9cdcfe>angle<span>)
Rotates the transform about axis passing through point in world coordinates by angle degrees.
#### void <span style="color":#dcdcaa>LookAt<span>([Vector3](../objects/Vector3.md) <span style="color":#9cdcfe>target<span>)
Rotates the transform so the forward vector points at worldPosition.
#### void <span style="color":#dcdcaa>SetRenderersEnabled<span>(bool <span style="color":#9cdcfe>enabled<span>)
Sets the enabled state of all child renderers.

---

