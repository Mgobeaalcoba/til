# Python 3.10+: @dataclass(slots=True)

Passing `slots=True` makes the dataclass use `__slots__`: less memory per instance and a typo in an attribute name raises `AttributeError` instead of silently creating a new attribute.

```python
from dataclasses import dataclass

@dataclass(slots=True)
class Point:
    x: float
    y: float
```
