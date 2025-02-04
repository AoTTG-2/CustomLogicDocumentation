# RacingCheckpointRegion

The RacingCheckpointRegion component refills human gas and sets the respawn point if the current game mode is racing.

```csharp
component RacingCheckpointRegion
{
    Refill = true;
    PlaySound = true;

    function OnCollisionEnter(other)
    {
        if (other.Type == "Human" && other.IsMine)
        {
            if (self.Refill)
            {
                other.RefillImmediate();
            }
            if (self.PlaySound)
            {
                other.PlaySound("Checkpoint");
            }
            other.Player.SpawnPoint = self.MapObject.Position;
        }
    }
}
```
