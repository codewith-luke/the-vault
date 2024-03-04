---
title: 03d - Performance & Optimization
tags:
  - aws
---
## Problem: Single PUT Upload

- When uploading it is a single data stream to S3 by *default*
- If the stream fails the upload fails
- This would require a full restart and can waste time and dependent on speed of connection
- Speed & reliability = limit of 1 stream
- Any upload is *limited to 5GB*

## Solution: Multipart Upload

- Data is broken up with a multi part upload
- The *min* data size *100mb* 
- This can be split to a *max* of 10,000 parts of 5MB to 5GB
- Last part can be smaller than 5MB
- Parts can fail and restarted
- Transfer rate = speeds of all the parts

## S3 Accelerated Transfer

The idea here is that when data is  transferred from one location to the other it may take an indirect route, in other words possibly not the most efficient. This is generally how the public internet path would be.

A solution to this is *transfer acceleration*. This uses AWS Edge Locations. The default is it is switched off. And has a couple of limitations:

- Bucket name cannot have periods 
- Must be DNS compatible 

This means when data is transferred it goes to the closest edge location. Which is still over the public internet, but a lot closer. This is all under the AWS global network. Which means a lot more direct communication.

![[Pasted image 20230928090233.png]]

## How to enable

1) Head to S3 and create a new bucket
	- Create a bucket without periods in the name
2) Head to properties and scroll to the bottom and turn on transfer acceleration
	- This creates a new endpoint to utilize the accelerated transfers

Below is a tool to show the difference in upload speeds. Which is based on your internet connection.

[http://s3-accelerate-speedtest.s3-accelerate.amazonaws.com/en/accelerate-speed-comparsion.html](http://s3-accelerate-speedtest.s3-accelerate.amazonaws.com/en/accelerate-speed-comparsion.html)