# Rigidbody

The Rigidbody component allows adding physics to a map object. Once added, you can use the SetVelocity and AddForce methods on the component to simulate physics, and GetVelocity to get the current velocity.

```csharp
component Rigidbody
{
    Mass = 1.0;
    Gravity = Vector3(0.0, -20.0, 0.0);
    FreezeRotation = false;
    Interpolate = false;

    function Init()
    {
        self.MapObject.AddBuiltinComponent("Rigidbody", self.Mass, self.Gravity, self.FreezeRotation, self.Interpolate);
    }

    function SetVelocity(velocity)
    {
        self.MapObject.UpdateBuiltinComponent("Rigidbody", "SetVelocity", velocity);
    }

    function AddForce(force)
    {
        self.MapObject.UpdateBuiltinComponent("Rigidbody", "AddForce", force);
    }

    function AddForceWithMode(force, mode)
    {
        self.MapObject.UpdateBuiltinComponent("Rigidbody", "AddForce", force, mode);
    }

    function AddForceWithModeAtPoint(force, point, mode)
    {
        self.MapObject.UpdateBuiltinComponent("Rigidbody", "AddForce", force, mode, point);
    }

    function AddTorque(force, mode)
    {
        self.MapObject.UpdateBuiltinComponent("Rigidbody", "AddTorque", force, mode);
    }

    function GetVelocity()
    {
        return self.MapObject.ReadBuiltinComponent("Rigidbody", "Velocity");
    }

    function GetAngularVelocity()
    {
        return self.MapObject.ReadBuiltinComponent("Rigidbody", "AngularVelocity");
    }
}
```
