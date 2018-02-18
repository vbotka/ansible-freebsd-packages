freebsd-packages
================

[![Build Status](https://travis-ci.org/vbotka/ansible-freebsd-packages.svg?branch=master)](https://travis-ci.org/vbotka/ansible-freebsd-packages)

[Ansible role](https://galaxy.ansible.com/vbotka/freebsd-packages/). Install and/or update packages at FreeBSD


Requirements
------------

None.


Variables
---------



Workflow
--------

1) Change shell to /bin/sh.

```
ansible host -e 'ansible_shell_type=csh ansible_shell_executable=/bin/csh' -a 'sudo pw usermod user -s /bin/sh'
```

2) Install role.

```
ansible-galaxy install vbotka.freebsd-packages
```

3) Fit variables.

```
~/.ansible/roles/vbotka.freebsd-packages/vars/main.yml
```

4) Create playbook.

```
> cat ~/.ansible/playbooks/freebsd-packages.yml
---
- hosts: example.com
  become: yes
  become_method: sudo
  roles:
    - role: vbotka.freebsd-packages
```

5) Configure the system.

```
ansible-playbook ~/.ansible/playbooks/freebsd-packages.yml
```

License
-------

[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)


Author Information
------------------

[Vladimir Botka](https://botka.link)


References
----------

- [FreeBSD handbook: 4.6.2. Configuring pkg Clients to Use a Poudriere Repository](https://www.freebsd.org/doc/handbook/ports-poudriere.html)
- [man pkg.conf](https://www.freebsd.org/cgi/man.cgi?query=pkg.conf&sektion=5)
