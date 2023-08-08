### Prerequisites

#### Disk

Usually refers to either **HDD (hard-disk drive)** or **SSD (solid-state drive)**. Data written to disk will persist through power failures and general machine crashes. Disk is also referred to as **non-volatile storage**.

SSD is far faster than HDD (see latencies of accessing data from SSD and HDD) but also far more expensive from a financial point of view. Because of that, HDD will typically be used for data that's rarely accessed or updated, but that's stored for a long time, and SSD will be used for data that's frequently accessed and updated.

#### Memory

Short for **Random Access Memory (RAM)**. Data stored in memory will be **lost** when the process that has written that data dies.

### Key Terms

## Latency

 The time it takes for a certain operation to complete in a system. Most often this measure is a time duration, like milliseconds or seconds. You should know these orders of magnitude:
 
-   Reading 1 MB from RAM: 250 μs (0.25 ms)
-   Reading 1 MB from SSD: 1,000 μs (1 ms)
-   Transfer 1 MB over Network: 10,000 μs (10 ms)
-   Reading 1MB from HDD: 20,000 μs (20 ms)
-   Inter-Continental Round Trip: 150,000 μs (150 ms)

![[Pasted image 20230506122244.png]]

## Throughput

The number of operations that a system can handle properly per time unit. For instance the throughput of a server can often be measured in requests per second (RPS or QPS).



![[Pasted image 20230506122405.png]]