sho
### Prerequisites

#### Reverse Proxy

A server that sits between clients and servers and acts on behalf of the servers, typically used for logging, load balancing, or caching.

## Key Terms

### Load Balancer

A type of reverse proxy that distributes traffic across servers. Load balancers can be found in many parts of a system, from the DNS layer all the way to the database layer.

### Server-Selection Strategy

How a load balancer chooses servers when distributing traffic amongst multiple servers. Commonly used strategies include round-robin, random selection, performance-based selection (choosing the server with the best performance metrics, like the fastest response time or the least amount of traffic), and IP-based routing.

### Hot Spot

When distributing a workload across a set of servers, that workload might be spread unevenly. This can happen if your sharding key or your hashing function are sub-optimal, or if your workload is naturally skewed: some servers will receive a lot more traffic than others, thus creating a "hot spot".

### Nginx

Pronounced "engine X"—not "N jinx", Nginx is a very popular web server that's often used as a reverse proxy and load balancer.

Learn more: [https://www.nginx.com/](https://www.nginx.com/)


![[Pasted image 20230506141854.png]]
