# Asset Bundles in Game

Once the asset bundle has been added to the map editor, you can place custom objects throughout the map. However, some steps need to be taken to make sure that other players can load these custom objects.

There are two options for allowing other players to load custom assets: sharing the asset bundle beforehand and instructing them to place it in their Documents/Aottg2/CustomAssets folder, or uploading the asset bundle to a remote file host and adding that link in the map editor.

To have players load the asset bundle locally, you must share the asset bundle file with them and have them move it to Documents/Aottg2/CustomAssets folder. After that they will be able to load the map as usual.

To have players load the asset bundle remotely, you must upload the asset bundle file to a web host, and then paste the URL to that file in the map editor. To do this, navigate to the map editor, and select Options -> Custom Assets to open the custom assets window. Then, paste the URL into the field next to the asset bundle name. Players will now be able to download the asset bundle when joining the room and loading the map for the first time.&#x20;

Note: The file name must be kept exactly the same as in the CustomAssets folder when uploading it to a web host, with no extensions. The URL must also be a direct download and not have any additional characters after the file name: for example, https://dropbox.com/user/example would be a valid URL as long as opening that will immediately download the file, while https://dropbox.com/user/example?dl=1 would not be. The URL must also directly download the asset bundle file, NOT a .zip or any other extensions.
