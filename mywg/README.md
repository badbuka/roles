My wireguard
=========

Role that sets up wireguard VPN on RH8(Rocky, Alma, Oracle etc).

### Variables
```
mywg_port: "465"            ## wireguard listen port
mywg_subnet: "10.0.0.1/24"  ## wireguard subnet
mywg_peers:                 ## list of peers to add
  - { name: "", public_key: "O00vX2z4O7RXULiK+Z83zoh3LPfpZCHkvQYYnLM8PQo=", allowed_ips: "10.0.0.2/32" }
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: mywg

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
