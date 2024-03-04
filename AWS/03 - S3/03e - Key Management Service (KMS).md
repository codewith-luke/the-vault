---
title: 03e - Key Management Service (KMS)
tags:
  - aws
---
## What is it?

AWS Key Management Service (AWS KMS) makes it easy for you to create and manage cryptographic keys and control their use across a wide range of AWS services and in your applications. AWS KMS is a secure and resilient service that uses hardware security modules that have been validated under FIPS 140-2, or are in the process of being validated, to protect your keys.

- Regional & Public Service
- Create, Store and Manage Keys
- Capable of *Symmetric* and *Asymmetric* Keys
- Can do cryptographic operations (*encrypt*, *decrypt*, etc)
- Keys never leave KMS (locked inside KMS)
	- It also complies with **FIPS 140-2 (Level2)**. An American security standard.

### How KMS Keys are made

- Think of them as containers of data securely
- KMS Keys are *logical* - ID, date, policy, desc & state
- Backed by physical key material to encrypt and decrypt
- KMS keys can be used for up to *4KB of data*
- You need the right permissions on the keys and in general in order to encrypt and decrypt. These are granular.

![[Pasted image 20231005113822.png]]

## Data Encryption Keys (DEK)

KMS does not do encryption on anything larger than 4KB. This is where you would do the encryption and decryption yourself and you would use a DEK.

![[Pasted image 20231005115239.png]]

## Key Concepts

- KMS Keys are isolated to a region & *never* leave (it does support multi-region)
- Can be AWS Owned & Customer Owned
- Customer managed keys are more configurable
- KMS Keys Support rotation
	- This will contain backing keys and previous backing keys
- Can create aliases to KMS keys (region locked based on key)

## Key Policies and Security

![[Pasted image 20231005120031.png]]

## How to

1) Head to KMS
2) Click create key (choose your key type and usage or advanced options)
3) Setup alias
4) Assign key admins
5) Then finish creating your key

### Using Key

1) Launch cloud shell
2) `echo "find all the doggos, distract them with the yumz" > battleplans.txt`
3) Encrypt
```
aws kms encrypt \
    --key-id alias/catrobot \
    --plaintext fileb://battleplans.txt \
    --output text \
    --query CiphertextBlob \
    | base64 --decode > not_battleplans.enc 
```
4) Decrypt
```
aws kms decrypt \
    --ciphertext-blob fileb://not_battleplans.enc \
    --output text \
    --query Plaintext | base64 --decode > decryptedplans.txt
```