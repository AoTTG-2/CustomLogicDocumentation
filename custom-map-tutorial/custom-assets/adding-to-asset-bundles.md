# Adding to Asset Bundles

To add content to the example asset bundle, first open the asset bundle project in Unity.

There should be a folder in the project called AssetBundle. This is where all custom assets should be placed. If you navigate to AssetBundle/Prefabs, you will find the only two prefabs in the project: ExampleCube.prefab and ExampleSphere.prefab. You can add more prefabs to this folder and they will show up as valid custom assets in the map editor.

Note that the custom asset system only supports adding custom prefabs to the map editor. Custom textures, materials, sounds, and animations can be added to the game, but only as part of a custom prefab.

IMPORTANT: If you are adding a prefab with a mesh, make sure the mesh object has the "Read/Write" flag enabled in the fbx or obj inspector.&#x20;

First create a new custom prefab in this folder. Next, you must assign it to be built to the asset bundle. To do this, select the new prefab, and in the bottom right you will see a "Asset Bundle: None" dropdown. Select the dropdown and change it to "example". Now the new prefab will be built into the same example asset bundle as the ExampleCube and ExampleSphere.&#x20;

Finally, build the asset bundle by right clicking the Assets folder and clicking Build AssetBundles. As in previous sections, you can now rename and move the resulting "example" file in the Builds folder to your CustomAssets folder.
