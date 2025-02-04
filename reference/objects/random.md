# Random

### Initialization

Random can be initialized as a class with a string given as the seed value.

Note that this is optional, and you can reference Random directly as a static class.

```python
# Create an instance of Random with a seed of 123
generator = Random(123);

# Use it
a = generator.RandomInt(0, 100);

# Seed allows repeatable random values
generator2 = Random(123);
b = generator.RandomInt(0, 100);

compared = a == b;    # Always True
```

### Methods

See [random.md](../static-classes/random.md "mention") for methods.

