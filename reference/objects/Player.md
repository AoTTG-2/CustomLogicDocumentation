# Player
Inherits from object
## Fields
|Field|Type|Readonly|Description|
|---|---|---|---|
|Character|[Character](../objects/Character.md)|False|Player's current character, if alive.|
|Connected|bool|False|Player is still connected to the room.|
|ID|int|False|Player unique ID.|
|Name|[String](../static/String.md)|False|Player name.|
|Guild|[String](../static/String.md)|False|Player guild.|
|Team|[String](../static/String.md)|False|Player's chosen team ("None", "Blue", "Red", "Titan", "Human"). Note that this may be different from the character's final team (Character.Team field) if the character's team field is modified.|
|Status|[String](../static/String.md)|False|Player's spawn status ("Alive", "Dead", "Spectating").|
|CharacterType|[String](../static/String.md)|False|Player's chosen character ("Human", "Titan", "Shifter")|
|Loadout|[String](../static/String.md)|False|Player's chosen loadout ("Blades", "AHSS", "APG", "Thunderspears").|
|Kills|int|False|Player's kills.|
|Deaths|int|False|Player's deaths.|
|HighestDamage|int|False|Player's highest damage.|
|TotalDamage|int|False|Player's total damage.|
|Ping|int|False|The player's connection ping.|
|SpectateID|int|False|The player's spectating ID. If not spectating anyone, returns -1.|
|SpawnPoint|[Vector3](../objects/Vector3.md)|False|Player's respawn point. Is initially null and can be set back to null, at which point map spawn points are used.|
## Methods
#### function <mark style="color:yellow;">GetCustomProperty</mark>(property: <mark style="color:blue;">[String](../static/String.md)</mark>) -> <mark style="color:blue;">Object</mark>
> Get a custom property at given key. Must be a primitive type. This is synced to all clients.

#### function <mark style="color:yellow;">SetCustomProperty</mark>(property: <mark style="color:blue;">[String](../static/String.md)</mark>, value: <mark style="color:blue;">Object</mark>) -> <mark style="color:blue;">void</mark>
> Sets a custom property at given key. Must be a primitive type. This is synced to all clients.

#### function <mark style="color:yellow;">ClearKDR</mark>() -> <mark style="color:blue;">void</mark>
> Clears kills, deaths, highestdamage, and totaldamage properties.


---

