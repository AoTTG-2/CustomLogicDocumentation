# Built-in Components Common Errors

When you add a component to an object, you may need to take into account what that component is doing/needs from the object it was placed on. Some components (especially those marked as internal) expect a certain set of properties to exist on the object. The cannon will expect some moveable parts to be defined in unity and the Wagon requires two wheel transforms and two empty gameobjects marking the boundary that characters can sit in. These components can be used alongside custom assets as long as you define the asset with the corresponding transforms/hierarchy.

Some other components expect animations, audio sources, or particle emitters. These must go on specific objects and more often than not, there should be map editor objects pre-filled out with their default component.

Another common case for errors is due to Object Attributes. If a component needs to move, scale, rotate, or change the color/texture properties, it must be marked as **not** `Static` and if it sends network messages through a `NetworkView` or needs its positioned synced in game, it must be marked as `Networked` . Please keep in mind to limit the number on Non-Static objects as they increase the number of [drawcalls ](https://docs.unity3d.com/Manual/optimizing-draw-calls.html)which will decrease the performance of your map.

If you have any questions about what is needed for setting up some built-in component, please first look for examples of their use in the built-in maps which can be viewed by selecting **File -> Load Preset** in the map editor. If you are unable to find an example or have another issue, please reach out via the Discord server as either people in the community or one of our developers will be glad to help you.
