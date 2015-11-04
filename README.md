# packer-install

Installs [Hasicorp's Packer](https://packer.io)



## Role Variables
```yml

---
packer:
  version: 0.8.6
  arch: amd64

install:
  dir : /usr/local/bin
  download_location: https://releases.hashicorp.com/packer/

```


Example Playbook
----------------
```yml

---
- hosts: local
  sudo: true
  gather_facts: true

  roles:
    - marcelocorreia.packer-install

  vars_files:
    - ../vars/tardis.yml

```

License
-------

MIT

Author Information
------------------
Some useful stuff at:
  - [https://github.com/marcelocorreia](https://github.com/marcelocorreia)
  - [https://galaxy.ansible.com/list#/users/15516](https://galaxy.ansible.com/list#/users/15516)
  - [https://hub.docker.com/u/marcelocorreia/](https://hub.docker.com/u/marcelocorreia/)
  - Any issues, pull-request are welcome
