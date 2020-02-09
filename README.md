Role Name
=========

bootstrap: install python

[![Build Status](https://travis-ci.org/cmihai-ansible/bootstrap.svg?branch=master)](https://travis-ci.org/cmihai-ansible/bootstrap)

Ansible galaxy:
---------------

[https://galaxy.ansible.com/devopstoolbox.bootstrap](https://galaxy.ansible.com/devopstoolbox.bootstrap)

```bash
ansible-galaxy install devopstoolbox.bootstrap
```

Requirements
------------

- For RHEL, a Red Hat subscription or functional local repository.

Role Variables
--------------

Dependencies
------------

- For Red Hat, subscription-manager.

Example Playbook
----------------

```yaml
---
- name: Install bootstrap on localhost
  hosts:
    - localhost
  connection: local
  gather_facts: false

  tasks:
    - name: bootstrap is configured
      import_role:
        name: devopstoolbox.bootstrap
      tags: bootstrap
```

License
-------

MIT

Author Information
------------------

- [Mihai Criveti](https://www.linkedin.com/in/crivetimihai)
