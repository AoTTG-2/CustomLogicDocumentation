# Range

Inherits from List. Allows you to create lists of integers for convenient iteration, particularly in for loops.

### Initialization

Range takes three ints Start, End (exclusive), and Step.

Example: Range(0, 10, 1) will return the list \[0, 1... 9], while Range(0, 10, 2) will return the list \[0, 2, 4... 8)

If Start > End and Step is negative, then the list will be in reverse order.

Example: Range(9, -1, -1) will return the list \[9, 8, 7... 0]
