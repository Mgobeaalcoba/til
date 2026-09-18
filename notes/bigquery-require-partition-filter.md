# BigQuery: force queries to filter on the partition column

Setting `require_partition_filter` on a partitioned table makes BigQuery reject any query that does not filter on the partitioning column. It is a cheap guardrail against accidental full-table scans.

```sql
ALTER TABLE mydataset.events
SET OPTIONS (require_partition_filter = TRUE);
```
