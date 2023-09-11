---
title: 02i - DNS Record Types
tags:
  - aws
---
## Nameserver

These are record types that allow delegation to occur in DNS.

![[Pasted image 20230903143136.png]]

## A & AAA Records

Given a DNS zone, these type of records map host names to IP addresses. You would generally create both A and AAA records and the client operating system or DNS software would then decide which would be used.

![[Pasted image 20230903143250.png]]

## CNAME Record

This stands for *Canonical Name*. This creates DNS shortcuts (host to host records). CNAME's cannot point to IP's, only other names.

![[Pasted image 20230903143543.png]]

## MX Records

MX Records in short are how a server can find a mail server for a specific domain. Whenever you send an email the server will be using DNS to do a MX lookup to find the mail server.

MX Records have 2 main parts:
- Priority
- Value

When it comes to value, the lower the value, the higher the priority. These values are used to determine when a MX Query comes in which record takes priority in resolving that query.

![[Pasted image 20230903144117.png]]
## TXT Records

Allow you to add text to a domain. A common usage is to prove domain ownership. Can also be used to fight spam.

![[Pasted image 20230903144307.png]]

## TTL - Time to Live

Is something that can be set on DNS records, numerical value in seconds. When a client makes a request to lets say amazon.com during the DNS resolve process when it reaches the **resolver server**, it is saying it will store the results for that set value in seconds, this is considered an **authoritative answer**. If another client makes a request it would then return a **non-authoritative answer**, however this will be immediate, as it was cached.


**![[Pasted image 20230903144525.png]]**