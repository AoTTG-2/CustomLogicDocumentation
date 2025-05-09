# SupplyStation

The SupplyStation component allows humans to refill gas and blades when in a certain region.

```csharp
component SupplyStation
{
    UnlimitedRefills = true;
    MaxRefills = 0;
    _currentHumanRefill = null;
    _currentHuman = null;

    function Init()
    {
        self._refillsLeft = self.MaxRefills;
        self.MapObject.AddBoxCollider("Region", "Characters", Vector3(0,-2,0), Vector3(14,8,14));
    }

    function OnCollisionStay(other)
    {
        if (other.Type == "Human" && other.IsMine && (self.UnlimitedRefills || self._refillsLeft > 0))
        {
            self._currentHuman = other;
            self._currentHumanRefill = other;
            UI.SetLabelForTime("MiddleCenter", "Press " + Input.GetKeyName("Interaction/Interact") + " to refill." + String.Newline + "Press " + Input.GetKeyName("Interaction/Interact2") + " to change loadout.", 0.1);
        }
    }

    function OnFrame()
    {
        if (self._currentHumanRefill != null)
        {
            if ((self._currentHumanRefill.AutoRefillGas || Input.GetKeyDown("Interaction/Interact")) && self._currentHumanRefill.Refill(true))
            {
                self._currentHumanRefill = null;
                self._refillsLeft = self._refillsLeft - 1;
            }
        }
        if (self._currentHuman != null)
        {
            if (Input.GetKeyDown("Interaction/Interact2"))
            {
                self._currentHuman = null;
                UI.ShowChangeCharacterMenu();
            }
        }
    }

    function OnCollisionExit(other)
    {
        if (other.Type == "Human" && other.IsMine)
        {
            self._currentHuman = null;
            self._currentHumanRefill = null;
        }
    }
}
```
