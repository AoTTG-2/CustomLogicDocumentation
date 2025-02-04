# Custom Logic Introduction

Aottg2 custom logic is a scripting language used for creating game modes. It features common language features such as classes, functions, as well as component bindings to map editor objects. Custom logic is a dynamically typed language, and is heavily designed around event callbacks to facilitate game mode design.

**Getting started:**\
Custom logic can be used in two ways: directly in the map editor, or as a separate game mode file. The first method will allow you to ship maps with logic already added, and the player will only need to select the map and the "Map Logic" game mode. The second method will allow you to use custom logic with any map (overriding any logic in the map itself), which is useful for sharing more generic game modes.

**Custom logic through map editor**\
To add custom logic to a custom map, in the map editor go to Options -> Custom Logic

Afterwards, paste your custom logic into the field and click Save. If the custom logic has parsing errors it will be displayed below the box. Now your custom logic is combined with the map, and when exported will be loaded alongside as long as players use the "Map Logic" game mode.

If your custom logic has custom components in the script, they can also now be added to map objects as components. To add a component, select a Map Object and click "Add Component" in the bottom right inspector. Here you can select script components and set their initial variables.

**Custom logic through file**

In the create game window, navigate to the "Custom" panel at the top right. Here you can import custom maps and custom logic as separate game modes. After importing your custom logic, it will now be selectable as a game mode when choosing any map.

Alternatively, you can add map and logic files directly by navigating to your Documents/Aottg2 folder. Here you can find the CustomLogic and CustomMap folders which can be edited directly.
