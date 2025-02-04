# Asset Bundle naming

In previous sections, our asset bundle was always called "example". However, it is highly recommended you apply unique names to your asset bundles to prevent conflicts with other map makers who may be deploying their own custom assets.&#x20;

To give your asset bundle a unique name, simply rename the "example" file before moving it to your CustomAssets folder or uploading it to a remote host. You can also create new asset bundle names in Unity by clicking "new" when assigning asset bundles to prefabs, but this is not required.&#x20;

An example of a good asset bundle name would be something like "MyUsernameCity1Assets". You should avoid using generic names like "CityAssets" or "Wagons".

Note that once asset bundles are named and loaded to the map editor, they cannot be renamed. Opening the map in the future will expect the same file name to be located in the CustomAssets folder. This also applies to custom prefab names - once you create a prefab called ExampleCube and place these objects in the map editor, it will expect the prefab to be the same name in the future.
