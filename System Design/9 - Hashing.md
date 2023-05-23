### Prerequisites

#### Hashing Function

A function that takes in a specific data type (such as a string or an identifier) and outputs a number. Different inputs _may_ have the same output, but a good hashing function attempts to minimize those **hashing collisions** (which is equivalent to maximizing **uniformity**).

#### Load Balancer

A type of **reverse proxy** that distributes traffic across servers. Load balancers can be found in many parts of a system, from the DNS layer all the way to the database layer.

### Key Terms

#### Consistent Hashing

A type of hashing that minimizes the number of keys that need to be remapped when a hash table gets resized. It's often used by load balancers to distribute traffic to servers; it minimizes the number of requests that get forwarded to different servers when new servers are added or when existing servers are brought down.

#### Rendezvous Hashing

A type of hashing also coined _highest random weight_ hashing. Allows for minimal re-distribution of mappings when a server goes down.
![[Pasted image 20230507140437.png]]

#### SHA

Short for "Secure Hash Algorithms", the SHA is a collection of cryptographic hash functions used in the industry. These days, SHA-3 is a popular choice to use in a system.
