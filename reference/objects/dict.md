# Dict

Inherits from Object. Dict (dictionaries) allow you to add and reference objects by key and value.

### Fields

<table><thead><tr><th width="175.33333333333331">Field</th><th width="122">Type</th><th width="108">Readonly</th><th>Description</th></tr></thead><tbody><tr><td>Keys</td><td>List(Object)</td><td>true</td><td>List of keys in the dictionary.</td></tr><tr><td>Values</td><td>List(Object)</td><td>true</td><td>List of values in the dictionary.</td></tr><tr><td>Count</td><td>int</td><td>true</td><td>Number of entries.</td></tr></tbody></table>

### Functions

<table><thead><tr><th>Function</th><th width="174.33333333333331">Returns</th><th>Description</th></tr></thead><tbody><tr><td>Clear</td><td>null</td><td>Clears the dictionary.</td></tr><tr><td>Get(key: Object, optional default: Object)</td><td>Object</td><td>Returns the value at given key. If the optional parameter default is provided, will return default if no key is found.</td></tr><tr><td>Set(key: Object, value: Object)</td><td>null</td><td>Sets the value at given key.</td></tr><tr><td>Remove(key: Object)</td><td>null</td><td>Removes the entry at given key.</td></tr><tr><td>Contains(key: Object)</td><td>bool</td><td>Whether or not the dictionary contains the key.</td></tr></tbody></table>
