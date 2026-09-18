# Python 3.10+: zip(strict=True)

`zip` silently stops at the shortest iterable. `strict=True` raises `ValueError` if the lengths differ, which catches misaligned data early.

```python
list(zip([1, 2, 3], ["a", "b"], strict=True))  # ValueError
```
