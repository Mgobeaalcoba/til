# SQL: avoid division by zero with NULLIF

`NULLIF(x, 0)` returns `NULL` when `x` is 0, and dividing by `NULL` yields `NULL` instead of an error.

```sql
SELECT revenue / NULLIF(orders, 0) AS avg_ticket
FROM daily_sales;
```

BigQuery also offers `SAFE_DIVIDE(revenue, orders)`.
