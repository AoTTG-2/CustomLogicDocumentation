# Network

Networking functions.

### **Fields**

<table><thead><tr><th width="174">Field</th><th width="137">Type</th><th width="121">Readonly</th><th>Description</th></tr></thead><tbody><tr><td>IsMasterClient</td><td>bool</td><td>true</td><td>Is current player the master client.</td></tr><tr><td>Players</td><td>List(Player)</td><td>true</td><td>List of all players in the room.</td></tr><tr><td>MasterClient</td><td>Player</td><td>true</td><td>The current master client.</td></tr><tr><td>MyPlayer</td><td>Player</td><td>true</td><td>My player.</td></tr><tr><td>NetworkTime</td><td>float</td><td>true</td><td>The current photon network time. This will probably be different from the Game time.</td></tr><tr><td>Ping</td><td>float</td><td>true</td><td>The current local player's ping.</td></tr></tbody></table>

### Functions

<table><thead><tr><th width="288">Function</th><th width="123.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>SendMessage(target: Player, message: string)</td><td>null</td><td>Send a network message to the target player. This will be received in the OnNetworkMessage callback in Main.</td></tr><tr><td>SendMessageAll(message: string)</td><td>null</td><td>Send a network message to all players including yourself.</td></tr><tr><td>SendMessageOthers(message: string)</td><td>null</td><td>Send a network message to all players excluding yourself.</td></tr><tr><td>GetTimestampDifference(float t1, float t2)</td><td>float</td><td>Compute the wrapped timestamp difference from photon events. Used to determine delay.</td></tr><tr><td>KickPlayer(player : Player|int, reason="")</td><td>null</td><td>Kick the player via ID or Player object from the room, only callable by the host.</td></tr></tbody></table>
