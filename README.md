# Role Name

A brief description of the role goes here.

## Requirements

```
docker run -p 8888:8888 -it --rm -v $PWD/:/tmp:Z cfssl/cfssl serve -address 0.0.0.0 -ca /tmp/ca.pem -ca-key /tmp/ca-key.pem
```

## Role Variables

See vars/main.yml

```
---
countryName:            "US"
localityName:           "New York"
organizationName:       "Your Organization Name"
organizationalUnitName: "Your Organizational Unit Name"
stateOrProvinceName:    "NY"
keySize:                2048
cfssl_hostname:         "127.0.0.1"
cfssl_port:             "8888"
```

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
- hosts: servers
  roles:
     - { role: username.rolename, x: 42 }
```

## License

BSD

## Author Information

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
