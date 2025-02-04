# PointLight

The PointLight component allows adding point lighting to a map. This creates light that comes from a point source with a specific range, rather than a global direction like Daylight.

```csharp
component PointLight
{
    Color = Color(255, 255, 255, 255);
    Intensity = 1.0;
    Range = 10.0;

    function Init()
    {
        self.MapObject.AddBuiltinComponent("PointLight", self.Color, self.Intensity, self.Range);
    }
}
```
