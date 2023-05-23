I am awful at this stuff. So there will be basic notes here.

- [[Useful Packages]]
- [[Useful Commands]]
- NVIM [[Notes]]

## Generating Self Signed Certificates

To start we can make use of the following .bash script to generate a self signed .cert and .key

```bash
#!/bin/bash

# Generate a self-signed certificate for a local development environment.
echo "Generating self-signed certificate..."
mkdir "./apps/server/cert"
openssl genrsa -out ./apps/server/cert/server.key 2048
openssl ecparam -genkey -name secp384r1 -out ./apps/server/cert/server.key
echo "Creating Cert..."
openssl req -new -x509 -sha256 -key ./apps/server/cert/server.key -out ./apps/server/cert/server.crt -batch -days 3650
```


Once that is done we then need to add that to the CA (Certificate Authority) on our system. To do that follow:

https://support.kerioconnect.gfi.com/hc/en-us/articles/360015200119-Adding-Trusted-Root-Certificates-to-the-Server

1.  To add: 
    1.  Copy your CA to `dir /usr/local/share/ca-certificates/`
    2.  Use command: `sudo cp foo.crt /usr/local/share/ca-certificates/foo.crt`
    3.  Update the CA store: `sudo update-ca-certificates`
2.  To remove:
    1.  Remove your CA.
    2.  Update the CA store: `sudo update-ca-certificates --fresh`


