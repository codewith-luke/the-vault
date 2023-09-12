## Overview

The role of the Death Star Auth is to provide a secure layer of access to Disclone. If someone finds a loophole. Were kinda f#$ked.

This service aims to provide the following:

- Username/Password logins
- Server side sessions
- Encrypted password storage
- Basic RBAC solution with different scopes
- Magic Link Login
- QR Code Login

**Tools:**
- Written in the [Bun](https://bun.sh/) runtime

## How it works

When logging in and registering new accounts against the Auth service this will do 2 things:

1) Create a x-session-id cookie
2) Create a x-signature cookie

The *session-id* is a long lived identifier that can be killed off in the server should we need to close off that session. Whereas the *x-signature* is a one time use token used to validate a request.