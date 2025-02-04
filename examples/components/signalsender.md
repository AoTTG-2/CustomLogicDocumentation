# SignalSender

Use in tandem with other compatible Signal components for specific operation and activation. Make sure the component has reverse enabled if needed.

```csharp
component SignalSender
{
    ReceiverObjectIDs = "0";
    SignalTrigger = "Any";
    ComponentName = "SignalMover";
    SetEasing = "Original";
    SetXYZ = Vector3(0, 0, 0);
    SetTimesPerSecond = 0.0;
    RepeatTimes = 1;
    SetInfinite = false;
    Uses = 0;
    InfiniteUses = true;
    OnStayTimer = 0.0;
    InteractDistance = 0;
    StopOnConstrains = false;
    ForwardOrReverse = "Both";

    Description = "Use in tandem with other compatible Signal components for specific operation and activation. Make sure the component has reverse enabled if needed.";
    ReceiverObjectIDsTooltip = "ID  for the receiving objects, use space to separate multiple receivers.";
    SignalTriggerTooltip = "How the signal is activated. (OnGetHit only works with cubes and Interact is not included for 'Any')";
    ComponentNameTooltip = "What component to send the signal to";
    SetXYZTooltip = "Only modifies original values if set to anything but (0, 0, 0)"
    SetTimesPerSecondTooltip = "Modify the speed value of target object, is ignored if value is 0";
    UsesTooltip = "How many times this signal can be used";
    StopOnConstrainsTooltip = "Receiver object will stop at start and end position. Use for things like doors.";
    ForwardOrReverseTooltip = "Whether the signal can only make the object go in one direction or both";
    OnStayTimerTooltip = "If OnCollisionStay trigger is selected. Will use the time input before signal is sent.";

    SetEasingDropbox = "Original, Linear, EaseIn, EaseOut, EaseInOut, BackIn, BackOut, BackInOut";
    SignalTriggerDropbox = "Any, OnCollisionEnter, OnCollisionStay, OnCollisionExit, OnGetHit, OnGetHooked, Interact";
    ComponentNameDropbox = "SignalArcMover, SignalMover, SignalRotator, SignalScaler";
    ForwardOrReverseDropbox = "Both, Forward, Reverse";

    _OnStayTimer = 0.0;
    _HumanInRange = null;

    _Receivers = List();
    _Components = List();
    function Init()
    {
        self._OnStayTimer = self.OnStayTimer;
        ReceiverIDs = String.Split(self.ReceiverObjectIDs, " ");
        for (i in Range(0, ReceiverIDs.Count, 1))
        {
            self._Receivers.Add(Map.FindMapObjectByID(Convert.ToInt(ReceiverIDs.Get(i))));
            self._Components.Add(self._Receivers.Get(i).GetComponent(self.ComponentName));
        }
        if (self.SignalTrigger == "OnGetHit" || self.SignalTrigger == "Any")
        {
            self.MapObject.AddBoxCollider("Physical", "Hitboxes", Vector3(0,self.MapObject.Scale.Y * 5, 0), Vector3(self.MapObject.Scale.X * 10,self.MapObject.Scale.Y * 10,self.MapObject.Scale.Z * 10));
        }
        if (self.SignalTrigger == "Interact")
        {
            self.MapObject.AddBoxCollider("Region", "Characters", Vector3(0,self.MapObject.Scale.Y * 5,0), Vector3(self.MapObject.Scale.X * 10 + self.InteractDistance,self.MapObject.Scale.Y * 10 + self.InteractDistance,self.MapObject.Scale.Z * 10 + self.InteractDistance));
        }
    }
    function OnCollisionEnter(other)
    {
        if (self.SignalTrigger == "OnCollisionEnter" || self.SignalTrigger == "Any")
        {
            for (i in Range(0, self._Receivers.Count, 1))
            {
                self.SendSignal(self._Receivers.Get(i), self._Components.Get(i));
            }
        }
    }
    function OnCollisionStay(other)
    {
        if (self.SignalTrigger == "OnCollisionStay" || self.SignalTrigger == "Any")
        {
            if (self._OnStayTimer <= 0.0)
            {
                for (i in Range(0, self._Receivers.Count, 1))
                {
                    self.SendSignal(self._Receivers.Get(i), self._Components.Get(i));
                }
            self._OnStayTimer = self.OnStayTimer;
            }
            else
            {
                self._OnStayTimer = self._OnStayTimer - Time.TickTime;
            }
        }
        if (self.SignalTrigger == "Interact" && other.Type == "Human" && other.IsMine && (self.Uses > 0 || self.InfiniteUses))
        {
            self._HumanInRange = other;
            UI.SetLabelForTime("MiddleCenter", "Press " + Input.GetKeyName("Interaction/Interact") + " to interact", 0.1);
        }
    }
    function OnCollisionExit(other)
    {
        self._OnStayTimer = self.OnStayTimer;
        self._HumanInRange = null;
        if (self.SignalTrigger == "OnCollisionExit" || self.SignalTrigger == "Any")
        {
            for (i in Range(0, self._Receivers.Count, 1))
            {
                self.SendSignal(self._Receivers.Get(i), self._Components.Get(i));
            }
        }
    }
    function OnGetHit(character, name, damage, type)
    {
        if (self.SignalTrigger == "OnGetHit" || self.SignalTrigger == "Any")
        {
            for (i in Range(0, self._Receivers.Count, 1))
            {
                self.SendSignal(self._Receivers.Get(i), self._Components.Get(i));
            }
        }
    }
    function OnGetHooked(Human, HookPos, LeftHook)
    {
        if (self.SignalTrigger == "OnGetHooked" || self.SignalTrigger == "Any")
        {
            for (i in Range(0, self._Receivers.Count, 1))
            {
                self.SendSignal(self._Receivers.Get(i), self._Components.Get(i));
            }
        }
    }
    function OnFrame()
    {
        if (self._HumanInRange != null)
        {
            if (Input.GetKeyDown("Interaction/Interact") && (self.Uses > 0 || self.InfiniteUses))
            {
                for (i in Range(0, self._Receivers.Count, 1))
                {
                    self.SendSignal(self._Receivers.Get(i), self._Components.Get(i));
                }
            }
        }
    }
    function SendSignal(Receiver, Component)
    {
        if ((self.Uses > 0 || self.InfiniteUses) && !Component._Running)
        {
            if (!self.InfiniteUses)
            {
                self.Uses = self.Uses - 1;
            }
            if (self.ComponentName == "SignalArcMover")
            {
                if (self.ForwardOrReverse == "Forward")
                {
                    if (Component.MapObject.Position != (Component._OriginalPosition + Component.TargetPosition) && self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ForwardTimes = self.RepeatTimes;
                    }
                    elif (!self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ForwardTimes = self.RepeatTimes;
                    }
                }
                elif (self.ForwardOrReverse == "Reverse")
                {
                    if (Component.MapObject.Position != Component._OriginalPosition && self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ReverseTimes = self.RepeatTimes;
                    }
                    elif (!self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ReverseTimes = self.RepeatTimes;
                    }
                }
                elif (self.ForwardOrReverse == "Both")
                {
                    Component.Activate = true;
                    Component._RepeatTimes = self.RepeatTimes;
                }
                if (Component.Activate)  
                {
                    if (self.SetXYZ != Vector3(0, 0, 0))
                    {
                        Component.TargetPosition = self.SetXYZ;
                    }
                    if (self.SetEasing != "Original")
                    {
                        Component.Easing = self.SetEasing;
                    }
                    if (self.SetTimesPerSecond != 0.0)
                    {
                        Component._TimesPerSecond = self.SetTimesPerSecond;
                    }
                    Receiver.Active = true;
                }
            }
            if (self.ComponentName == "SignalMover")
            {
                if (self.ForwardOrReverse == "Forward")
                {
                    if (Component.MapObject.Position != (Component._OriginalPosition + Component.TargetPosition) && self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ForwardTimes = self.RepeatTimes;
                    }
                    elif (!self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ForwardTimes = self.RepeatTimes;
                    }
                }
                elif (self.ForwardOrReverse == "Reverse")
                {
                    if (Component.MapObject.Position != Component._OriginalPosition && self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ReverseTimes = self.RepeatTimes;
                    }
                    elif (!self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ReverseTimes = self.RepeatTimes;
                    }
                }
                elif (self.ForwardOrReverse == "Both")
                {
                    Component.Activate = true;
                    Component._RepeatTimes = self.RepeatTimes;
                }
                if (Component.Activate)  
                {
                    if (self.SetXYZ != Vector3(0, 0, 0))
                    {
                        Component.TargetPosition = self.SetXYZ;
                    }
                    if (self.SetEasing != "Original")
                    {
                        Component.Easing = self.SetEasing;
                    }
                    if (self.SetTimesPerSecond != 0.0)
                    {
                        Component._TimesPerSecond = self.SetTimesPerSecond;
                    }
                    Receiver.Active = true;
                }
            }
            elif (self.ComponentName == "SignalRotator")
            {
                if (self.ForwardOrReverse == "Forward")
                {
                    if (Component.MapObject.Rotation != (Component._OriginalRotation + Component.Rotation) && self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ForwardTimes = self.RepeatTimes;
                    }
                    elif (!self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ForwardTimes = self.RepeatTimes;
                    }
                }
                elif (self.ForwardOrReverse == "Reverse")
                {
                    if (Component.MapObject.Rotation != Component._OriginalRotation && self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ReverseTimes = self.RepeatTimes;
                    }
                    elif (!self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ReverseTimes = self.RepeatTimes;
                    }
                }
                elif (self.ForwardOrReverse == "Both")
                {
                    Component.Activate = true;
                    Component._RepeatTimes = self.RepeatTimes;
                }
                if (Component.Activate)  
                {
                    if (self.SetXYZ != Vector3(0, 0, 0))
                    {
                        Component.Rotation = self.SetXYZ;
                    }
                    if (self.SetEasing != "Original")
                    {
                        Component.Easing = self.SetEasing;
                    }
                    if (self.SetTimesPerSecond != 0.0)
                    {
                        Component._TimesPerSecond = self.SetTimesPerSecond;
                    }
                    Receiver.Active = true;
                }   
            }
            elif (self.ComponentName == "SignalScaler")
            {
                if (self.ForwardOrReverse == "Forward")
                {
                    if (Component.MapObject.Scale != Vector3.Multiply(Component._OriginalScale, Component.MultiplyScale) && self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ForwardTimes = self.RepeatTimes;
                    }
                    elif (!self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ForwardTimes = self.RepeatTimes;
                    }
                }
                elif (self.ForwardOrReverse == "Reverse")
                {
                    if (Component.MapObject.Scale != Component._OriginalScale && self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ReverseTimes = self.RepeatTimes;
                    }
                    elif (!self.StopOnConstrains)
                    {
                        Component.Activate = true;
                        Component._ReverseTimes = self.RepeatTimes;
                    }
                }
                elif (self.ForwardOrReverse == "Both")
                {
                    Component.Activate = true;
                    Component._RepeatTimes = self.RepeatTimes;
                }
                if (Component.Activate)  
                {
                    if (self.SetXYZ != Vector3(0, 0, 0))
                    {
                        Component.MultiplyScale = self.SetXYZ;
                    }
                    if (self.SetEasing != "Original")
                    {
                        Component.Easing = self.SetEasing;
                    }
                    if (self.SetTimesPerSecond != 0.0)
                    {
                        Component._TimesPerSecond = self.SetTimesPerSecond;
                    }
                    Receiver.Active = true;
                }
            }
        }
    }  
}
```
