### Prerequisites

#### Client

A machine or process that requests data or service from a server.

Note that a single machine or piece of software can be both a client and a server at the same time. For instance, a single machine could act as a server for end users and as a client for a database.

#### Server

A machine or process that provides data or service for a client, usually by listening for incoming network calls.

Note that a single machine or piece of software can be both a client and a server at the same time. For instance, a single machine could act as a server for end users and as a client for a database.

#### IP Address

An address given to each machine connected to the public internet. IPv4 addresses consist of four numbers separated by dots: `a.b.c.d` where all four numbers are between 0 and 255. Special values include:

- `127.0.0.1`: Your own local machine. Also referred to as `localhost`.
- `192.168.x.y`: Your private network. For instance, your machine and all machines on your private wifi network will usually have the `192.168` prefix.

## Key Terms

#### IP

Stands for **Internet Protocol**. This network protocol outlines how almost all machine-to-machine communications should happen in the world. Other protocols like **TCP**, **UDP** and **HTTP** are built on top of IP.

#### TCP

Network protocol built on top of the Internet Protocol (IP). Allows for ordered, reliable data delivery between machines over the public internet by creating a **connection**.

TCP is usually implemented in the kernel, which exposes **sockets** to applications that they can use to stream data through an open connection.

#### HTTP

The **H**yper**T**ext **T**ransfer **P**rotocol is a very common network protocol implemented on top of TCP. Clients make HTTP requests, and servers respond with a response.

**Requests typically have the following schema:**

```
host: string (example: example.io)
port: integer (example: 80 or 443)
method: string (example: GET, PUT, POST, DELETE, OPTIONS or PATCH)
headers: <key, value=""> pair list (example: "Content-Type" => "application/json")
body: opaque sequence of bytes
```

**Responses typically have the following schema:**

```
status code: integer (example: 200, 401)
headers: <key, value=""> pair list (example: "Content-Length" => 1238)
body: opaque sequence of bytes
```

#### IP Packet

Sometimes more broadly referred to as just a (network) **packet**, an IP packet is effectively the smallest unit used to describe data being sent over **IP**, aside from bytes. An IP packet consists of:

- an **IP header**, which contains the source and destination **IP addresses** as well as other information related to the network
- a **payload**, which is just the data being sent over the network