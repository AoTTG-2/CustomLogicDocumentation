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
#### <span style="color:blue;">[Transform](../objects/Transform.md)</span> <span style="color:yellow;">GetTransform</span>(<span style="color:blue;">[String](../static/String.md)</span> name)
> Gets the transform of the specified child.
#### <span style="color:blue;">[List](../objects/List.md)</span> <span style="color:yellow;">GetTransforms</span>()
> Gets all child transforms.
#### <span style="color:blue;">void</span> <span style="color:yellow;">PlayAnimation</span>(<span style="color:blue;">[String](../static/String.md)</span> anim, <span style="color:blue;">float</span> fade = <span style="color:blue;">0.1</span>)
> Plays the specified animation.
#### <span style="color:blue;">float</span> <span style="color:yellow;">GetAnimationLength</span>(<span style="color:blue;">[String](../static/String.md)</span> anim)
> Gets the length of the specified animation.
#### <span style="color:blue;">void</span> <span style="color:yellow;">PlaySound</span>()
> Plays the sound.
#### <span style="color:blue;">void</span> <span style="color:yellow;">StopSound</span>()
> Stops the sound.
#### <span style="color:blue;">void</span> <span style="color:yellow;">ToggleParticle</span>(<span style="color:blue;">bool</span> enabled)
> Toggles the particle system.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">InverseTransformDirection</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> direction)
> Transforms a direction from world space to local space. The opposite of Transform.TransformDirection.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">InverseTransformPoint</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> point)
> Transforms position from world space to local space.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">TransformDirection</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> direction)
> Transforms direction from local space to world space.
#### <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> <span style="color:yellow;">TransformPoint</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> point)
> Transforms position from local space to world space.
#### <span style="color:blue;">void</span> <span style="color:yellow;">Rotate</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> rotation)
> Applies a rotation of eulerAngles.z degrees around the z-axis, eulerAngles.x degrees around the x-axis, and eulerAngles.y degrees around the y-axis (in that order).
#### <span style="color:blue;">void</span> <span style="color:yellow;">RotateAround</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> point, <span style="color:blue;">[Vector3](../objects/Vector3.md)</span> axis, <span style="color:blue;">float</span> angle)
> Rotates the transform about axis passing through point in world coordinates by angle degrees.
#### <span style="color:blue;">void</span> <span style="color:yellow;">LookAt</span>(<span style="color:blue;">[Vector3](../objects/Vector3.md)</span> target)
> Rotates the transform so the forward vector points at worldPosition.
#### <span style="color:blue;">void</span> <span style="color:yellow;">SetRenderersEnabled</span>(<span style="color:blue;">bool</span> enabled)
> Sets the enabled state of all child renderers.

---

