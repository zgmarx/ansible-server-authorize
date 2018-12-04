ansible-server-authorize
==========

Key based authentication in SSH is called public key authentication.

By apply this role, you will "Add the content of id_rsa.pub to remote servers(ansible client) authorized_keys".

Then you could login target host without password.

Usage
-----

```
---
- hosts: localhost
  connection: local
  roles:
    - role: ansible-server-authorize
      usedns: "UseDNS no"
      gssapi: false
```
