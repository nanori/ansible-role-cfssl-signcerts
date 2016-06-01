# Ansible role for automated certificate signing with cfssl

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

```
- hosts: localhost
  roles:
     - { role: ansible-role-cfssl-signcerts, hostname: 'foo.bar.example.com' }
```

## License

## Author Information
