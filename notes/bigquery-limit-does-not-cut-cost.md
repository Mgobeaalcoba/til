# BigQuery: LIMIT does not reduce the bytes scanned

Adding `LIMIT` to a query limits the rows returned, but on an unclustered table the query still scans (and bills) every selected column over the data it reads.

To actually cut cost: select only the columns you need and filter on the partition column.
