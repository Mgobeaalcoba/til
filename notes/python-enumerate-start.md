# Python: enumerate(start=1)

`enumerate` accepts a `start` argument, handy for human-friendly numbering such as row numbers in a report.

```python
for i, row in enumerate(rows, start=1):
    print(i, row)
```
