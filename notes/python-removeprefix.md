# Python 3.9+: removeprefix vs lstrip

`lstrip` takes a *set of characters*, not a prefix. `removeprefix` removes an exact prefix, once.

```python
"toto-x".lstrip("to")        # '-x'
"toto-x".removeprefix("to")  # 'to-x'
```
