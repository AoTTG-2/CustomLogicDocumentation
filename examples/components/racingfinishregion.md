# RacingFinishRegion

The RacingFinishRegion component finishes the race if the current gamemode is Racing.

```csharp
component RacingFinishRegion
{
    function OnCollisionEnter(other)
    {
        if (other.Type == "Human" && other.IsMine)
        {
            Main.FinishRace(other);
        }
    }
}
```
