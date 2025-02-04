# Daylight

The Daylight component allows adding directional lighting to a map.

```csharp
component Daylight
{
    Color = Color(255, 255, 255, 255);
    Intensity = 1.0;
    WeatherControlled = true;

    function Init()
    {
        self.MapObject.AddBuiltinComponent("Daylight", self.Color, self.Intensity, self.WeatherControlled);
    }
}
```
