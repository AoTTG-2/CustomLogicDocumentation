# Components

These callback functions are available only on components. Components also have all the callbacks that exist in Main.

<table><thead><tr><th width="300">Function</th><th>Description</th><th data-hidden></th></tr></thead><tbody><tr><td>OnCollisionEnter(other: Object)</td><td>Called upon another object first colliding with the attached MapObject.</td><td></td></tr><tr><td>OnCollisionStay(other: Object)</td><td>Called every frame while another object is colliding with the attached MapObject.</td><td></td></tr><tr><td>OnCollisionExit(other: Object)</td><td>Called upon another object exiting collision with the attached MapObject.</td><td></td></tr><tr><td>OnGetHit(character: Character, name: string, damage: int, type: string, hitPosition: Vector3)</td><td>Called upon getting hit by a hitbox, such as a blade or titan attack. Only called if the MapObject has a collider of layer "Hitboxes" attached.</td><td></td></tr><tr><td>OnGetHooked(human: Human, hookPosition: Vector3, leftHook: bool)</td><td>Called upon getting hit by a hook. Only runs for your player character.</td><td></td></tr></tbody></table>

### **Network callbacks**

The following callbacks are only available if the attached MapObject has the "Networked" option enabled in the map editor.&#x20;

<table><thead><tr><th width="279">Function</th><th>Description</th></tr></thead><tbody><tr><td>OnNetworkTransfer(oldOwner: Player, newOwner: Player)</td><td>Called upon the NetworkView changing ownership.</td></tr><tr><td>SendNetworkStream()</td><td>Called every frame for the owner. You can send a series of data, in order, by using self.NetworkView.SendStream.</td></tr><tr><td>OnNetworkStream()</td><td>Called every frame for every non-owner observer. You can receive the series of data, in order, by using self.NetworkView.ReceiveStream.</td></tr><tr><td>OnNetworkMessage(sender: Player, message: string)</td><td>Called upon receiving a self.NetworkView.SendMessage call.</td></tr></tbody></table>

Note that the OnNetworkMessage callback is separate from the one in Main:  Main receives messages from the Network.SendMessage call, while components receive their own channel messages from the self.NetworkView.SendMessage call.
