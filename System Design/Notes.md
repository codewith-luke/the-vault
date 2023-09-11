1. Consider using a Cache for read-heavy systems.  
2. For low latency, use a Cache & CDN.  
3. Utilize a Message Queue for async processing in write-heavy systems.  
4. Choose an RDBMS or SQL Database for ACID compliance.  
5. Opt for a No-SQL Database for unstructured data without ACID requirements.  
6. Use Blob/Object storage for systems with complex data like videos, images, files, etc.  
7. Employ a Message Queue & Cache for systems with complex pre-computation tasks like a news feed.  
8. Use a search index, tries, or a search engine (like Elasticsearch) for high-volume data searching.  
9. Consider Database Sharding for scaling SQL Databases.  
10. Use a Load Balancer for High Availability, Performance, & Throughput.  
11. Employ a CDN for faster global data delivery, reliability, high availability, & performance. 
12. Choose a Graph Database for systems with data involving nodes, edges, and relationships.  
13. Implement Horizontal Scaling for scaling various components (servers, databases, etc.). 
14. Utilize Database Indexes for high-performing database queries.  
15. Use Batch Processing & Message Queues for bulk job processing.  
16. Employ a Rate Limiter to reduce server load and prevent DOS attacks.  
17. Consider using an API Gateway (Authentication, SSL Termination, Routing, etc.) for systems with microservices.  
18. Implement Redundancy for components with a single point of failure.  
19. Implement Data Replication (creating multiple copies of data on different servers) for fault tolerance and durability.  
20. Use Websockets for fast, bi-directional user-to-user communication.  
21. Implement a Heartbeat mechanism for detecting failures in distributed systems.  
22. Ensure data integrity using a Checksum Algorithm.  
23. Implement Consistent Hashing to efficiently scale servers with node add/removal and avoid hotspots.  
24. Use Gossip Protocol for decentralized data transfer between servers.  
25. Utilize Quadtree, Geohash, etc., for location-based functionalities like maps and nearby resources.  
26. Prefer generic names like message queues, object storage, etc., instead of specific technology names.  
27. Mention that a system with High Availability cannot have strong consistency; eventual consistency is possible.  
28. Explain DNS (Domain Name System) when discussing how domain name queries resolve IP addresses in browsers.  
29. Implement Pagination to limit response data for network requests with a large amount of data.  
30. Use LRU (Least Recently Used) Cache eviction policy and understand its Data Structure and Implementation.