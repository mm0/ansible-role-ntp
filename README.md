Ansible Role: NTP v1.0
===

[![Build Status](https://travis-ci.org/mm0/ansible-role-ntp.svg?branch=master)](https://travis-ci.org/mm0/ansible-role-ntp)

An Ansible role that installs and re-configures NTP daemon with your list of servers

See Also: ansible-role-directory


Requirements
---

None 

Role Variables
---

Available variables are listed below, along with values defaults to AWS servers:

```yml
ntp_servers: 
    - server 0.amazon.pool.ntp.org iburst
    - server 1.amazon.pool.ntp.org iburst
    - server 2.amazon.pool.ntp.org iburst
    - server 3.amazon.pool.ntp.org iburst
```

Dependencies
---

None 

Example Playbook
---

```yml
- hosts: webservers
  roles:
  - { role: ansible-role-ntp }
```

License
---------------

BSD-2

Author Information
------------------

[Matt Margolin](mailto:matt.margolin@gmail.com)

[mm0](https://github.com/mm0) on github