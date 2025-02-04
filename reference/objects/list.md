# List

Inherits from Object. Lists allow you to keep an ordered array of objects.

### Fields

<table><thead><tr><th width="175.33333333333331">Field</th><th width="122">Type</th><th width="108">Readonly</th><th>Description</th></tr></thead><tbody><tr><td>Count</td><td>int</td><td>true</td><td>Number of items.</td></tr></tbody></table>

### Functions

<table><thead><tr><th width="290">Function</th><th width="110.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>Clear</td><td>null</td><td>Clears the list.</td></tr><tr><td>Get(index: int)</td><td>Object</td><td>Returns the item at given index.</td></tr><tr><td>Set(index: int, item: Object)</td><td>null</td><td>Sets the item at given index.</td></tr><tr><td>Add(item: Object)</td><td>null</td><td>Adds an item to the end of the list.</td></tr><tr><td>InsertAt(index: int, item: Object)</td><td>null</td><td>Inserts an item at the given index.</td></tr><tr><td>RemoveAt(index: int)</td><td>null</td><td>Removes the item at the given index.</td></tr><tr><td>Remove(item: Object)</td><td>null</td><td>Removes the item from the list.</td></tr><tr><td>Contains(item: Object)</td><td>bool</td><td>Returns true if the item is contained in the list.</td></tr><tr><td>Sort</td><td>null</td><td>Sorts the items in the list in place if the items are comparable (int, float, string).</td></tr><tr><td>Randomize</td><td>null</td><td>Randomizes the list order.</td></tr></tbody></table>

