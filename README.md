klems.install-resilio
=========
[![Build Status](https://travis-ci.org/klems/ansible-role-install-resilio.svg?branch=master)](https://travis-ci.org/klems/ansible-role-install-resilio)

A role to install resilio sync (formerly bittorent sync)

Requirements
------------
Ansible == `2.4`

Role Variables
--------------
### {{ resilio_folders }}
A list of folders that will be created as resilio root folders with rslsync user ownership.

```
resilio_folders:
  - /mnt/storage-01
  - /mnt/storage-02
```

Dependencies
------------
N/A

Example Playbook
----------------
```
- hosts: servers
  roles:
     - { role: klems.install-resilio, resilio_folders: ['/mnt/storage-01', '/mnt/storage-02'] }
```

License
-------
BSD

Author Information
------------------
mail: klems@klems.net
