PIP
==========

Install a list of PyPi packages.

Requirements
------------

 - None

Role Variables
---------------

```yaml
---
pip_packages:
  - pkg1
  - pkg2
  - name: pkg3
    version: 2.1.0

```

Dependencies
------------

 - None

Example Playbook
----------------

```yaml
---
- hosts: webapp
  vars:
    pip_packages:
      - jinja2
      - name: celery
        version: 3.1.0
      - paramiko
  roles:
    - role: apt

```

License
-------

MIT
