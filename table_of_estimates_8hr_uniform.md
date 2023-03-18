To estimate the requests per second for various number of users sending messages per hour, assuming uniform traffic for 8 hours, refer to the table below for baseline numbers:

| Messages per Hour | Users | Total Messages | Requests per Second | Requests per Minute | Requests per Hour |
| --- | --- | --- | --- | --- | --- |
| 2 | 1000 | 16000 | 0.005 | 0.3 | 18 |
| 2 | 1000000 | 16000000 | 5.56 | 333.3 | 20000 |
| 2 | 1000000000 | 16000000000 | 5555.56 | 333333.3 | 20000000 |
| 5 | 1000 | 40000 | 0.012 | 0.7 | 42 |
| 5 | 1000000 | 40000000 | 13.89 | 833.3 | 50000 |
| 5 | 1000000000 | 40000000000 | 13888.89 | 833333.3 | 50000000 |
| 10 | 1000 | 80000 | 0.024 | 1.4 | 84 |
| 10 | 1000000 | 80000000 | 27.78 | 1667 | 100000 |
| 10 | 1000000000 | 80000000000 | 27777.78 | 1666667 | 100000000 |

### Message size: 10 bytes

| Messages per Hour | Users | Total Messages | Requests per Second | Requests per Minute | Requests per Hour | Throughput (10-byte messages) |
| --- | --- | --- | --- | --- | --- | --- |
| 2 | 1000 | 16000 | 0.0016 | 0.096 | 5.76 | 160 bytes/s |
| 5 | 1000 | 40000 | 0.003 | 0.18 | 10.8 | 300 bytes/s |
| 10 | 1000 | 80000 | 0.0048 | 0.288 | 17.28 | 480 bytes/s |

### Message size: 1 KB

| Messages per Hour | Users | Total Messages | Requests per Second | Requests per Minute | Requests per Hour | Throughput (1 KB messages) |
| --- | --- | --- | --- | --- | --- | --- |
| 2 | 1000 | 16000 | 0.00002 | 0.0012 | 0.072 | 20 KB/s |
| 5 | 1000 | 40000 | 0.00005 | 0.003 | 0.18 | 50 KB/s |
| 10 | 1000 | 80000 | 0.0001 | 0.006 | 0.36 | 100 KB/s |

| Messages per Hour | Users | Total Messages | Requests per Second | Requests per Minute | Requests per Hour | Throughput (1 MB messages) |
| --- | --- | --- | --- | --- | --- | --- |
| 2 | 1000 | 16000 | 0.00000002 | 0.0000012 | 0.000072 | 20 MB/s |
| 5 | 1000 | 40000 | 0.00000005 | 0.000003 | 0.00018 | 50 MB/s |
| 10 | 1000 | 80000 | 0.0000001 | 0.000006 | 0.00036 | 100 MB/s |