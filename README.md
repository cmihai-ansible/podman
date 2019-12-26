Role Name
=========

podman

[![Build Status](https://travis-ci.org/cmihai-ansible/podman.svg?branch=master)](https://travis-ci.org/cmihai-ansible/podman)

Ansible galaxy:
---------------

[https://galaxy.ansible.com/crivetimihai/podman(https://galaxy.ansible.com/crivetimihai/podman)

```bash
ansible-galaxy install crivetimihai.podman
```

Requirements
------------

- For RHEL, a Red Hat subscription or functional local repository.

Role Variables
--------------

```
podman_remove_packages: true
```

Dependencies
------------

- For Red Hat, subscription-manager.

Example Playbook
----------------

```yaml
---
- name: Install podman on localhost
  hosts:
    - localhost
  connection: local

  tasks:
    - name: podman is configured
      import_role:
        name: crivetimihai.podman
      vars:
        podman_remove_packages: true
      tags: podman
```

License
-------

MIT

Author Information
------------------

- [Mihai Criveti](https://www.linkedin.com/in/crivetimihai/)
