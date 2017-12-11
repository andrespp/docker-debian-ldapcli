Docker phpVirtualBox
====================

# Introduction

DockerFile for Debian with ldap authentication

This image is based on `FROM debian:jessie`.

# Quick start

```bash
$ docker container run --rm -it -v $(pwd)/libnss-ldap.conf:/etc/libnss-ldap.conf:ro andrespp/debian-ldapcli bash
```

Where `./libnss-ldap.conf` is like:

```
base dc=base
uri ldap://192.168.1.1/
ldap_version 3
binddn uid=linux,ou=system,dc=base
bindpw secret-password
```


# Available variables

Todo 
