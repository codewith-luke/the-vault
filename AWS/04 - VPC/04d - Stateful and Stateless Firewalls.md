---
title: 04d - Stateful and Stateless Firewalls
tags:
  - aws
---

The below image shows the common way of thinking how a client connects to a server. However in reality what actually happens is a little different. Take a look at the diagram below to get a better understanding of how a HTTPS connection actually would occur.

![[Pasted image 20231109083721.png]]

By understanding the real full flow of packets we can then understand the next diagram around if a request/response is considered *INBOUND* or *OUTBOUND* in the case of firewall rules. This has to do with perspective. In the sense of if you are the client sending a request, that is outbound, while a server receiving would be inbound (then visa versa).

![[Pasted image 20231109084246.png]]

## Stateless Firewall

As the name suggests. A stateless firewall means it does not understand the state of connections. Meaning it sees the request and response as 2 individual parts. So you would need 2 rules in order to manage this. 

![[Pasted image 20231109084608.png]]

When considering rules always consider the direction of the request. As the response will always be the inverse.

![[Pasted image 20231109084836.png]]

## Stateful Firewalls

This is a firewall that is intelligent enough to identify the request and response are related to a connection. Therefore you would only need to have a single rule, reducing admin overhead and possibility for mistakes.

![[Pasted image 20231109085254.png]]