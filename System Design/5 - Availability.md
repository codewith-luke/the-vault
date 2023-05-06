### Prerequisites

### Process

A program that is currently running on a machine. You should always assume that any process may get terminated at any time in a sufficiently large system.

### Server

A machine or process that provides data or service for a client, usually by listening for incoming network calls. Note that a single machine or piece of software can be both a client and a server at the same time. For instance, a single machine could act as a server for end users and as a client for a database.

### Node/Instance/Host

These three terms refer to the same thing most of the time: a virtual or physical machine on which the developer runs processes. Sometimes the word server also refers to this same concept.

## Key Terms

## Availability

The odds of a particular server or service being up and running at any point in time, usually measured in percentages. A server that has 99% availability will be operational 99% of the time (this would be described as having two **nines** of availability).

## High Availability

Used to describe systems that have particularly high levels of availability, typically 5 nines or more; sometimes abbreviated "HA".

## Nines

Typically refers to percentages of uptime. For example, 5 nines of availability means an uptime of 99.999% of the time. Below are the downtimes expected per year depending on those 9s:

-   99% (two 9s): 87.7 hours
-   99.9% (three 9s): 8.8 hours
-   99.99%: 52.6 minutes
-   99.999%: 5.3 minutes

## Redundancy

The process of replicating parts of a system in an effort to make it more reliable.

## SLA

Short for "service-level agreement", an SLA is a collection of guarantees given to a customer by a service provider. SLAs typically make guarantees on a system's availability, amongst other things. SLAs are made up of one or multiple SLOs.

## SLO

Short for "service-level objective", an SLO is a guarantee given to a customer by a service provider. SLOs typically make guarantees on a system's availability, amongst other things. SLOs constitute an SLA.