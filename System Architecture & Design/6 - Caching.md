### Prerequisites

### Latency 

The time it takes for a certain operation to complete in a system. Most often this measure is a time duration, like milliseconds or seconds. You should know these orders of magnitude:

-   **Reading 1 MB from RAM**: 250 μs (0.25 ms)
-   **Reading 1 MB from SSD**: 1,000 μs (1 ms)
-   **Transfer 1 MB over Network**: 10,000 μs (10 ms)
-   **Reading 1MB from HDD**: 20,000 μs (20 ms)
-   **Inter-Continental Round Trip**: 150,000 μs (150 ms)
-   Throughput

The number of operations that a system can handle properly per time unit. For instance the throughput of a server can often be measured in requests per second (RPS or QPS).

-   Memory

Short for **Random Access Memory (RAM)**. Data stored in memory will be lost when the process that has written that data dies.

### Key Terms

#### Cache

A piece of hardware or software that stores data, typically meant to retrieve that data faster than otherwise.

Caches are often used to store responses to network requests as well as results of computationally-long operations.

Note that data in a cache can become **stale** if the main source of truth for that data (i.e., the main database behind the cache) gets updated and the cache doesn't.

#### Cache Hit

When requested data is found in a cache.

#### Cache Miss

When requested data could have been found in a cache but isn't. This is typically used to refer to a negative consequence of a system failure or of a poor design choice. For example:

_If a server goes down, our load balancer will have to forward requests to a new server, which will result in cache misses._

#### Cache Eviction Policy

The policy by which values get evicted or removed from a cache. Popular cache eviction policies include **LRU** (least-recently used), **FIFO** (first in first out), and **LFU** (least-frequently used).

#### Content Delivery Network

A **CDN** is a third-party service that acts like a cache for your servers. Sometimes, web applications can be slow for users in a particular region if your servers are located only in another region. A CDN has servers all around the world, meaning that the latency to a CDN's servers will almost always be far better than the latency to your servers. A CDN's servers are often referred to as **PoPs** (Points of Presence). Two of the most popular CDNs are **Cloudflare** and **Google Cloud CDN**.