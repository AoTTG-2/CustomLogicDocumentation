# Object Attributes

When you select an object, the right-hand inspector panel shows up which allows you to change some attributes of the object.

**Active:** Whether the object begins activated or not. If disabled, the object will be disabled at the start of the game.

**Static:** Whether the object will remain static (no position, rotation, scaling, or visibility changes) or not. If you plan on moving the object through custom logic or components, or changing its visibility or active state, then this toggle should be disabled. Otherwise, if the object will never move or change visibility, enabling this toggle improves performance.

**Networked:** Whether this object requires certain custom logic networking features, such as syncing states or movement. If you add any custom logic component that requires network sync, or if you add movement that you prefer to keep synced on multiplayer, then you should enable this toggle.

**Name:** The name of this object as it appears in the object list panel and in custom logic.

**Parent Id:** The parent of this object, based on Object Id (found at the top left of the inspector panel). If you set a parent for this object, it will follow the parent's movements and rotations.

**Position:** The X, Y, and Z values of the object position.

**Rotation:** The X, Y, and Z values of the object rotation.

**Scale:** The X, Y, and Z values of the object scale.

**Collide Mode:** How the object should collide with other objects. Use None for no collision, Physical for normal collisions, and Region for region collisions. Region collisions are also known as triggers, and are often used by custom scripts to detect collisions without creating a physical barrier. Note that region colliders are only available for geometry objects.

**Collide With:** What types of objects the object will collide with. Use All for everything, MapObjects for other map objects, Projectiles for projectiles such as hooks, thunderspears, and cannonballs, Characters for characters such as Humans and Titans, and Entities for characters and projectiles.

**Physics Material:** The physics material attached to the object.

**Visible:** Whether or not the object will be visible in-game.

**Shader:** What kind of material shader to use on the object. Use Default for the default material with an optional color tint, DefaultNoTint for the default material but using the default material color instead of tinting, Basic for a basic material that accepts a texture and tiling, and Transparent for a basic material that also has an alpha channel.&#x20;

**Components:** You can add additional component scripts by using the Add Component button at the bottom. For example, add the DamageRegion component to make the object damage characters upon collision.



