ageres210784.sysctl
=========

Ansible role to install and configure/reconfigure sysctl.

Requirements
------------

Ansible 2.1+

Role Variables
--------------

Set variable sysctl_settings  
Example:
```yml
sysctl_settings:
  net.ipv4.ip_forward: 1
```

Dependencies
------------

None

Example Playbook
----------------

```yml
- hosts: servers
  become: true
  roles:
      - { role: ageres210784.sysctl, tags ['sysctl'] }
```

License
-------

Apache-2.0

Author Information
------------------

This role was created by [Evseev Sergey](https://github.com/Ageres210784)
