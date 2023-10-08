# ansible-role-docker
Simple ansible role for configure docker on a remote machine

This role require [ansible-common-role](https://github.com/stethewwolf/ansible-common-role).

## Packages installed
This role install the following packages on the target
```
  - docker.io
  - python3
  - python3-pip
  - python3-setuptools
  - python3-docker
```

## Configuration

This role profide this congiuration parameter :

```
portainer_enable: false //if set as `true` install portainer
portainer_disable_firewall: false //if set as `true` open portainer port to all networks
```
Portainer container will:
* will have access to docker socker
* use the host network
* exopose the port 9000

## References
* [docker]()
* [portainer]()
