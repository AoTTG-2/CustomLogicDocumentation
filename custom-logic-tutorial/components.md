# Components

Components are a type of class that can be added to map objects through the map editor. They have access to the callback functions Main has, as well as some unique ones such as collisions and network events.

Once components are declared and the custom logic is loaded into the map editor, they can be added to objects via the "Add Component" button in the inspector window.

```csharp
component DamageRegion
{
    Damage = 100;

    function OnCollisionEnter(other)
    {
        if (other.IsCharacter && other.IsMine)
        {
            other.GetDamaged("Server", self.Damage);
        }
    }
}
```

OnCollisionEnter is a callback function unique components that gets called whenever the map object enters collision with another object. Here we deal 100 damage to any character that collides with the map object.&#x20;

The Damage variable will also be visible in the map editor and can be modified in the inspector to a custom value, allowing for different map objects to have a custom Damage value.
