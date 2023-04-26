# Table of Content
[[1 - Resources Management]]
[[2 - Swarm MTLS]]
[[3 - Content Trust]]
[[4 - Groups]]
[[5 - Container Capabilities]]
[[6 - Privileged Containers]]

Here is a good resource for a 'checklist' of things for security.
https://cheatsheetseries.owasp.org/cheatsheets/Docker_Security_Cheat_Sheet.html

## Image Scanning

Docker Trusted Registry (DTR) is a commercial product that enables organizations to store and manage their Docker images securely on-premises or in the cloud. It provides features such as image signing, vulnerability scanning, and auditing, to help ensure the security and integrity of images in the registry. DTR is integrated with Docker Enterprise and is available as an add-on for Docker Enterprise and Docker Community Edition.

There are other sorts of image scanning services available. However the main responsibility of these is to check for any vulnerabilities and issues.

## UCP

Docker Universal Control Plane (UCP) is a commercial product that provides a graphical user interface and a set of tools for managing and deploying Docker containers in a cluster. UCP integrates with Docker Enterprise and allows administrators to create and manage Docker networks, services, and containers, as well as configure security and access control policies. UCP also provides tools for monitoring and logging the status and performance of containers and services, and allows users to deploy and manage applications using a web-based dashboard or a command-line interface.

Docker UCP also provides tools for monitoring and logging the status and performance of containers, as well as managing access control and security policies. This allows organizations to ensure that their containers are running efficiently and securely in the cluster.

## LDAP

LDAP (Lightweight Directory Access Protocol) is a standard protocol for accessing and managing directory services over a network. Directory services are databases that store information about users, groups, and other resources in an organization, such as network devices and applications. LDAP provides a set of operations for querying and modifying the directory, such as searching for entries, adding or deleting entries, and modifying attributes. LDAP also defines a hierarchical structure for organizing entries in the directory, and uses a simple, human-readable syntax for representing entries and their attributes. LDAP is commonly used for authentication and authorization, to manage access to network resources and applications. It is also used for storing and sharing other types of information, such as contact lists and organizational data.
