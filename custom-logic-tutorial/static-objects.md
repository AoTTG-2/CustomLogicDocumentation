# Static Objects

In the map editor, you will notice a "Static" checkbox on each map object. This denotes whether the object will ever move, change active status, or change visibility. If you intend on modifying objects using Custom Logic, you must disable the Static attribute. Likewise if you don't need an object to move or change visibility, you should enable the Static attribute so that the object can benefit from static batching optimization.

By default all objects are static unless the checkbox is disabled.
