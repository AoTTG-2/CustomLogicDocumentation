# Cutscene

Cutscene functions.

<table><thead><tr><th width="271">Function</th><th width="101.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>Start(name: string, full: bool)</td><td>null</td><td>Starts cutscene with name. If full is true, will enter cinematic mode. Otherwise will only show dialogue while still allowing gameplay.</td></tr><tr><td>ShowDialogue(icon: string, title: string, content: string)</td><td>null</td><td>Show dialogue screen with given icon, title, and content. Available icons are the same as profile icon names.</td></tr><tr><td>ShowDialogueForTime(icon: string, title: string, content: string, time: float)</td><td>null</td><td>Show dialogue screen and automatically hide after <code>time</code> seconds.</td></tr><tr><td>HideDialogue()</td><td>null</td><td>Hides the dialogue screen.</td></tr></tbody></table>

For more detailed cutscenes, you can use the Camera class to control the camera.
