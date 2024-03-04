---
title: 05c - Storage
tags:
  - aws
---
## Types of Storage

- **Direct** (local) attached storage - storage on the EC2 Host
	- **Ephemeral** storage - temporary storage
- **Network** attached storage - Volumes delivered over the network (EBS)
	- **Persistent** storage - Permanent storage - live on past the life time of the instance

### Categories of Storage

- **Block** storage - **Volume** presented to the OS as a collection of blocks. No structure provided (*mountable, bootable*)
- **File** storage - Presented as a file share (has structure). (*mountable, NOT bootable*)
- **Object** storage - Collection of objects (flat) (*NOT mountable, NOT bootable*)

## Performance

![[Pasted image 20231212085739.png]]

## EBS
### What is it?

Amazon Elastic Block Store (Amazon EBS) provides block level storage volumes for use with EC2 instances. EBS volumes behave like raw, unformatted block devices. You can mount these volumes as devices on your instances. EBS volumes that are attached to an instance are exposed as storage volumes that persist independently from the life of the instance. You can create a file system on top of these volumes, or use them in any way you would use a block device (such as a hard drive).

- **Block** storage - raw disk alllocations (**volume**) - Can be encrypted using **KMS**
- Instances see block device and create a file system on this device
- Storage is provisioned in **ONE AZ** (resilient in that AZ)
- Attached to *ONE* EC2 instance  (or other service) over a storage network
	- They can be detached from one to another instance, but should consider it as 1to1
- Can snapshot (backup) to S3. Create volume from snapshot (migrate between AZs)
- EBS can provision volumes based on different physical storage *types, sizes or performance profiles*
- Billed base on *GB per month* (and in some cases performance)

### Basic Use of EBS

![[Pasted image 20231213085030.png]]

Main thing to note on the above is that you **CANNOT** share a EBS cross AZ or region. It is AZ locked. 

### Types of EBS
### GP2 (General Purpose Default SSD)

- Works on a credit architecture anything less than 1000GB

![[Pasted image 20231213085713.png]]

### GP3 (New General Purpose SSD)

- Doesn't use the credit architecture, is more simple

![[Pasted image 20231213090036.png]]

### Provisioned IOPS SSD (io1 and io2)

*Note: Make sure you know what an IO credit is.

![[Pasted image 20231213090821.png]]

### HDD Based

- Slower but there could be scenarios you would want to use

![[Pasted image 20231213091254.png]]

### EBS Snapshots

- Snapshots are incremental volume copies to S3
- The first is a full copy of 'data' on the volume
- Future snapshots are incremental (meaning they only store the difference)
- Volumes can be created/restored from snapshots

#### EBS Snapshots/Volume Performance

- New EBS Volume = full performance immediately
- Snaps restore lazily - fetched gradually
- Requested blocked are fetched immediately
- Force a read of all data immediately
- Fast Snapshot Restore (FSR) - Immediate restore
	- Up to 50 snaps per region. Set on the Snap & AZ

![[Pasted image 20231214085109.png]]
## Instance Store Volumes

- Provide **Block Storage** devices
- Physically connected to *one EC2 host*
	- Instance on that host can access them
- Highest storage performance in AWS
- Included in the instance price
- **ATTACHED AT LAUNCH**
	- Can't add new ones
- More IOPS and Throughput vs EBS
	- D3 Instances can get = 4.6 GB/s throughput
	- I3 Instances can get = 16GB GB/s of sequential throughput

![[Pasted image 20231213154836.png]]

![[Pasted image 20231213155225.png]]

#### Good to know on Instance Store Volumes

- Local on EC2 Host (if it dies you lose that data)
- Launch time only (have to add it before)
- Lost on instance move, resize or hardware failure
- High performance
- Payed for in the price of an instance
- TEMPORARY - always remember this

## Choosing between Instance Store and EBS

#### **Instance Store Volumes**

Use when you need:
- Super high performance
- Cost
- When you don't need persistence

The important distinction when it comes to instance store is that when you stop and start a EC2 instance which is an operation which would move the EC2 instance. This as a result would mean that it would be on different hardware, so your instance store would not persist. Comparing this to restarting an EC2 instance which would still use the same hardware, and so the instance store would persist.
#### **EBS**

Use when you need:
- You require persistence 
- Resilience
- Storage isolated from instance lifecycle

When talking about cost in EBS:
- Cheap = ST1 or SC1 (mechanical storage)

When talking about throughput or streaming:
- ST1

If there is mention of boot you cannot use:
- ST1 or SC1

When talking about key performance levels:
- GPT2/3 deliver up to *16 000 IOPS*
- IO1/2 - up to 64 000 IOPS (*256 000 for IO2 block express*)
- All the above has to be paired with a good EC2 instance to get the performance
- Can create a **RAID0** set + EBS up to 260 000 IPS (IO1/2-BE/GP2/3)
	- 260 000 is the *maximum* possible IOPS for an instance
- If you need more than the max you need to then consider [[#Instance Store Volumes]]

#### **It Depends?**

Use when you need:
- Resilience with app in-built replication
- High performance


## EBS Encryption

### How it works

When not using encryption for your volume it would be stored as plain text at rest. However when it comes to encryption this would make use of a KMS key (the default would be using *aws/ebs* as we are dealing with the EBS service). So when creating an encrypted volume this will have a DEK that will be used on the EC2 Host for encryption/decryption. 

This key would be decrypted and stored in memory on the EC2 Host (if the EC2 moves from this host it is *discarded*), on a new host the DEK would needs to decrypted and loaded into the new host. This then allows for data flowing from the EC2 instance through the host to then encrypt and store that data inside the volume (encrypted at rest).

### Useful notes

- Accounts can be set to encrypt by default - default KMS key
	- Otherwise choose a key to use
- Each volume uses *1 unique DEK*
- Snapshots & future volumes use the *same DEK*
- You cannot change a volume to be *NOT* encrypted
- OS isn't aware of the encryption, no performance loss

## Creating EBS Volumes

*Note: with the below example it would be based off the one click deployment from [here](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?templateURL=https://learn-cantrill-labs.s3.amazonaws.com/awscoursedemos/0004-aws-associate-ec2-ebs-demo/A4L_VPC_3PUBLICINSTANCES_AL2023.yaml&stackName=EBSDEMO)*
*Full YAML found [here](https://learn-cantrill-labs.s3.amazonaws.com/awscoursedemos/0004-aws-associate-ec2-ebs-demo/A4L_VPC_3PUBLICINSTANCES_AL2023.yaml)

Any commands we reference can be found [here](https://learn-cantrill-labs.s3.amazonaws.com/awscoursedemos/0004-aws-associate-ec2-ebs-demo/lesson_commands_AL2023.txt)

1. Deploy the demo from the first link (you can also setup your own EC2 instances)
	 - This will create us 3 EC2 instances
 2. Head over to EC2 instances and you should have at least a single instance running
	 1. Navigate to volume and select create volume
	 2. Select GP3
	 3. Select your AZ
	 4. Add a tag to identify your volume
	 5. Create
	 6. When available you can then attach to instance
 3. Select your volume and then attach volume
 4. Connect to your instance
	 1. Check that your can view block devices `lsblk`
	 2. Check your device has a file system `sudo file -s /dev/${device}`
		 - If this returns something like `data` then it means we need to create the file system
	 3. If you need to create file system run `sudo mkfs -t xfs /dev/${device}`
	 4. We then make a folder to mount our volume to `sudo mkdir /ebstest`
	 5. Then mount `sudo mount /dev/${device} /ebstest`
	 6. Check this with `df -k` to validate



This in a nutshell, is you cannot rely on instance stores to keep your data safe. It is ephemeral.
#### Setting up EBS Volume File System

1. First we need to shut down our instance and reconnect. As we do not have automounting enabled for this when running `df -k` it would not should our mounted volume.
2. Run `sudo blkid` and we should see our volume */dev/xvdf*
	-  Copy the identifier
3. Run `sudo vi /etc/fstab` (This is the configuration file for which file systems are mounted by our instance)
	- With your copied identifier add a new line with `UUID=${id} /ebstest xfs defaults,nofail`
	- Save and exit
4. Run `sudo mount -a` then use `df -k` to check that it has mounted
5. Now if we have disconnected our volume and attached it to a new instance when we type `lsblk` to check available storage we can see our *xvdf* volume.
	1. Type `sudo file -s /dev/xvdf` and it should show that it has a file system
	2. Make a new directory for us to mount this volume to
		1. `sudo mkdir /ebtest`
		2. `sudo mount /dev/xvdf /ebtest`
		3. `cd /ebtest`
		4. `ls -la`
#### Creating Snapshots of Volumes

1. Right click your volume and click *Create Snapshot*
2. Add description and create
3. Head to snapshots tab and wait for it to be created
4. When created you can now right click and create volume from your snapshot (this is because it is actually stored in S3). This means you can make it in a new AZ.
5. Once the volume is created in correct AZ you can then attach volume to an instance. Here you can now follow *step 5* from [[#Setting up EBS Volume File System]]

