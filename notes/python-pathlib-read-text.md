# Python: Path.read_text

`pathlib.Path` can read a small file in one line and closes it for you. Always pass the encoding explicitly.

```python
from pathlib import Path

text = Path("data.txt").read_text(encoding="utf-8")
```
