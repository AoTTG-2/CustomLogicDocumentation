# MovePingPong

The MovePingPong component moves an object between two positions. If RelativePositions is false, it will use the world position instead of the local position.

```csharp
component MovePingPong
{
    RelativePositions = true;
    StartPosition = Vector3(0, 0, 0);
    EndPosition = Vector3(0, 0, 0);
    Speed = 10.0;
    PauseTime = 0.0;
    _currentProgress = 0.0;
    _backwards = false;
    _pauseTimeLeft = 0.0;

    function Init()
    {
        if (self.RelativePositions)
        {
            self.StartPosition = self.MapObject.Position + self.StartPosition;
            self.EndPosition = self.MapObject.Position + self.EndPosition;
        }

        distance = Vector3.Distance(self.StartPosition, self.EndPosition);
        self._step = 1.0;
        if (distance > 0)
        {
            self._step = self.Speed / distance;
        }
    }

    function OnTick()
    {
        if (self._pauseTimeLeft > 0)
        {
            self._pauseTimeLeft = self._pauseTimeLeft - Time.TickTime;
            return;
        }
        if (self._backwards)
        {
            self._currentProgress = self._currentProgress - Time.TickTime * self._step;
            if (self._currentProgress <= 0.0)
            {
                self._currentProgress = 0.0;
                self._backwards = false;
                self._pauseTimeLeft = self.PauseTime;
            }
            self.MapObject.Position = Vector3.Lerp(self.StartPosition, self.EndPosition, self._currentProgress);
        }
        else
        {
            self._currentProgress = self._currentProgress + Time.TickTime * self._step;
            if (self._currentProgress >= 1.0)
            {
                self._currentProgress = 1.0;
                self._backwards = true;
                self._pauseTimeLeft = self.PauseTime;
            }
            self.MapObject.Position = Vector3.Lerp(self.StartPosition, self.EndPosition, self._currentProgress);
        }
    }
}
```
