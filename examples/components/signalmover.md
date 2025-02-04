# SignalMover

This and all other Signal\<Action> components are useful for more complicated animated movement. You can use the SignalSender activating the SignalMover. (Ex: Setting a trigger with Signal Sender that when hit kicks off a SignalMover)

When using this component, please mark the object as Networked and not Static.

```csharp
component SignalMover
{
    Activate = true;
    Reverse = false;
    Easing = "Linear";
    ReverseFlipsCurve = false;
    TargetPosition = Vector3(0,0,0);
    TimesPerSecond = 1.0;
    RepeatTimes = 0;
    Infinite = true;
    Interpolate = false;
    
    Description = "Moves the object. Activate auto-disables after operation is done, re-send signal to restart. Use SignalSender component if Modular use is necessary.";
    ActivateTooltip = "Enable to start operation. Counts as 1 repeat time.";
    ReverseTooltip = "Returns to original position after Target movement.";
    ReverseFlipsCurveTooltip = "If reverse is enabled, this alternates the easing for the In/Out counterparts. Does nothing for InOut or Linear.";
    InterpolateTooltip = "Smoothens movement using frames. Avoid unless necessary.";
    InfiniteTooltip = "Infinitely moves while activated, regardless of Repeat times.";
    TimesPerSecondTooltip = "The speed of the operation.";
    RepeatTimesTooltip = "How many operations will be done.";
    EasingTooltip = "The type of weight to apply to the animation.";

    EasingDropbox = "Linear, EaseIn, EaseOut, EaseInOut, BackIn, BackOut, BackInOut";

    _StartPosition = Vector3(0,0,0);
    _GoalPosition = Vector3(0,0,0);
    _OriginalPosition = Vector3(0,0,0);

    _Forwards = true;
    _Running = false;
    _TimesPerSecond = 0.0;
    _TickTimer = 0.0;
    _FrameTimer = 0.0;
    _XTime = 0.0;
    _RepeatTimes = 0;
    _ForwardTimes = 0;
    _ReverseTimes = 0;

    function Init()
    {
        self._OriginalPosition = self.MapObject.Position;
        self._StartPosition = self.MapObject.Position;
        self._GoalPosition = self.MapObject.Position + self.TargetPosition;
        self._RepeatTimes = self.RepeatTimes;
        self._TimesPerSecond = self.TimesPerSecond;
    }
    function OnTick()
    {   
        if (!Network.IsMasterClient)
        {
            return;
        }
        if ((self.Infinite || self._RepeatTimes > 0 || self._ForwardTimes > 0 || self._ReverseTimes > 0) && self.Activate && !self._Running)
        {
            self._Running = true;
            if (self._ForwardTimes > 0)
            {
                self._StartPosition = self.MapObject.Position;
                self._GoalPosition = self._StartPosition + self.TargetPosition;
                self._ForwardTimes = self._ForwardTimes - 1;
            }
            elif (self._ReverseTimes > 0)
            {
                self._StartPosition = self.MapObject.Position;
                self._GoalPosition = self._StartPosition - self.TargetPosition;
                self._ReverseTimes = self._ReverseTimes - 1;
            }
            elif (self.Infinite || self._RepeatTimes > 0)
            {
                if (!self.Infinite)
                {
                    self._RepeatTimes = self._RepeatTimes - 1;
                }
                if (self._Forwards)
                {
                    self._Forwards = false;
                    self._StartPosition = self.MapObject.Position;
                    self._GoalPosition = self._StartPosition + self.TargetPosition;
                }
                elif (!self._Forwards && self.Reverse == true)
                {
                    self._Forwards = true;
                    self._StartPosition = self.MapObject.Position;
                    self._GoalPosition = self._StartPosition - self.TargetPosition;
                    if (self.ReverseFlipsCurve)
                    {
                        self.Easing = ReverseEasing(self.Easing);
                    }
                }
                elif (!self._Forwards && self.Reverse == false)
                {
                    self._StartPosition = self.MapObject.Position;
                    self._GoalPosition = self._StartPosition + self.TargetPosition;
                }
            }
        }
        elif (!self.Infinite && self._RepeatTimes == 0 && self._ForwardTimes == 0 && self._ReverseTimes == 0 && !self._Running)
        {
            self.Activate = false;
            self._TimesPerSecond = self.TimesPerSecond;
        }

        if (self._Running && !self.Interpolate && self._TickTimer < (0.99 / self._TimesPerSecond))
        {
            self._TickTimer = self._TickTimer + Time.TickTime;
            XTime = self._TickTimer * self._TimesPerSecond;
            self.Calculate(XTime);
        }
        elif (self._Running && !self.Interpolate)
        {
            self._TickTimer = 0.0;
            self._Running = false;
            self.MapObject.Position = self._GoalPosition;
        }
    }
    function OnFrame()
    {
        if (!Network.IsMasterClient)
        {
            return;
        }
        if (self._Running && self.Interpolate && self._FrameTimer < (0.998 / self._TimesPerSecond))
        {
            self._FrameTimer = self._FrameTimer + Time.FrameTime;
            XTime = self._FrameTimer * self._TimesPerSecond;
            self.Calculate(XTime);
        }
        elif (self._Running && self.Interpolate)
        {
            self._FrameTimer = 0.0;
            self._Running = false;
            self.MapObject.Position = self._GoalPosition;
        }
    }
    function ReverseEasing(Easing)
    {
    if (Easing == "EaseIn")
    {
        Easing = "EaseOut";
    }
    elif (Easing == "EaseOut")
    {
        Easing = "EaseIn";
    }
    elif (Easing == "BackIn")
    {
        Easing = "BackOut";
    }
    elif (Easing == "BackOut")
    {
        Easing = "BackIn";
    }
    return Easing;
    }
    function Calculate(XTime)
    {    
        if (!Network.IsMasterClient)
        {
            return;
        }
        #Easing handling
        c1 = 1.70158;
        c2 = c1 * 1.525;
        c3 = c1 + 1;
        if (self.Easing == "Linear")
        {
            self.MapObject.Position = Vector3.Lerp(self._StartPosition, self._GoalPosition, XTime);
        }
        elif (self.Easing == "EaseIn")
        {
            self.MapObject.Position = Vector3.Lerp(self._StartPosition, self._GoalPosition, Math.Pow(XTime , 3));
        }
        elif (self.Easing == "EaseOut")
        {
            self.MapObject.Position = Vector3.Lerp(self._StartPosition, self._GoalPosition, 1 - Math.Pow(1 - XTime, 3));
        }
        elif (self.Easing == "EaseInOut")
        {
            if (XTime < 0.5)
            {
                XTime = 4 * XTime * XTime * XTime;
            }
            elif (XTime >= 0.5)
            {
                XTime = 1 - Math.Pow(-2 * XTime + 2, 3) / 2;
            }
            self.MapObject.Position = Vector3.Lerp(self._StartPosition, self._GoalPosition, XTime);
        }
        elif (self.Easing == "BackIn")
        {
            XTime = c3 * XTime * XTime * XTime - c1 * XTime * XTime;
            self.MapObject.Position = Vector3.LerpUnclamped(self._StartPosition, self._GoalPosition, XTime);
        }
        elif (self.Easing == "BackOut")
        {
            XTime = 1 + c3 * Math.Pow(XTime - 1, 3) + c1 * Math.Pow(XTime - 1, 2);
            self.MapObject.Position = Vector3.LerpUnclamped(self._StartPosition, self._GoalPosition, XTime);
        }
        elif (self.Easing == "BackInOut")
        {
            if (XTime < 0.5)
            {
                XTime = (Math.Pow(2 * XTime, 2) * ((c2 + 1) * 2 * XTime - c2)) / 2;
            }
            elif (XTime >= 0.5)
            {
                XTime = (Math.Pow(2 * XTime - 2, 2) * ((c2 + 1) * (XTime * 2 - 2) + c2) + 2) / 2;
            }
            self.MapObject.Position = Vector3.LerpUnclamped(self._StartPosition, self._GoalPosition, XTime);
        }
    }
}
```
