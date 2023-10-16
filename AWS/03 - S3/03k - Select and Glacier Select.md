---
title: 03k - Select and Glacier Select
tags:
  - aws
---
## What is it?

S3 can store huge objects (5TB), of which you often want to retrieve the entire object. But t retrieving large objects takes time, and filtering on the client side *doesn't* reduce it.

In S3/Glacier provide services that allow you to access partial objects, through *SQL like* statements. Which allows you to select part of the object, *pre-filtered by S3* (CSV, JSON, Parquet, BZIP2 Compression for CSV and JSON).

![[Pasted image 20231009160212.png]]
