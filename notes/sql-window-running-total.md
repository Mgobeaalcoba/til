# SQL: running total with a window function

A cumulative sum is a `SUM` with an ordered window, no self-join needed.

```sql
SELECT day,
       amount,
       SUM(amount) OVER (ORDER BY day) AS running_total
FROM daily_sales;
```
