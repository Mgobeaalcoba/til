# BigQuery: dedupe with QUALIFY

`QUALIFY` filters on the result of a window function, so keeping the latest row per key needs no subquery.

```sql
SELECT *
FROM `project.dataset.users`
WHERE TRUE
QUALIFY ROW_NUMBER() OVER (PARTITION BY user_id ORDER BY updated_at DESC) = 1;
```

BigQuery expects a `WHERE`, `GROUP BY` or `HAVING` next to `QUALIFY`, so `WHERE TRUE` is a common placeholder.
