# Python 3.9+: functools.cache

`functools.cache` is a shortcut for `lru_cache(maxsize=None)`: an unbounded memoization cache. Arguments must be hashable, and the cache grows forever, so use `lru_cache(maxsize=...)` for long-lived processes.

```python
from functools import cache

@cache
def fib(n: int) -> int:
    return n if n < 2 else fib(n - 1) + fib(n - 2)
```
