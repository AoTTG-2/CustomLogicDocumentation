# Networking

In the map editor, you will notice a "Networked" checkbox on each map object. This denotes whether the object will be using Custom Logic networking functions such as NetworkVIew and OnNetwork or OnStream callbacks. In order to mark an object for sync and networking, you must enable the "Networked" attribute. Afterwards, the NetworkView object becomes available for access in the custom logic component (via self.NetworkView), and the following network callbacks become available: SendNetworkStream, OnNetworkStream, OnNetworkMessage.
