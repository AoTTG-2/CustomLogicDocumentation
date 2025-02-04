# Asset Bundles in Map Editor

In the previous section we created an asset bundle named "example". First, make sure this file is moved to the Documents/Aottg2/CustomAssets folder. This is where the game looks for all custom assets.

Next, open the map editor, and select Options -> Custom Assets. This will bring up the custom asset menu where you can select which asset bundles are loaded for this specific map.

To register our custom asset bundle to the map, type in the asset bundle name (in this case "example") and click Add. The asset bundle is now loaded into the map editor, and its custom prefabs can now be added as objects in the Add Object -> Custom tab.&#x20;

The example asset bundle has two custom prefabs called ExampleCube and ExampleSphere that should now show up in the AddObject -> Custom tab. You can then add and place these objects like any other object in the map editor.

Note that the map now depends on this asset bundle file with this same name to be present in the CustomAssets folder in order to be opened and edited in the future. If you share this map with others, be sure to include the asset bundle and instruct them to place it in the CustomAssets folder.
