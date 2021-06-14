# freebsd_packages

[![quality](https://img.shields.io/ansible/quality/27910)](https://galaxy.ansible.com/vbotka/freebsd_packages)[![Build Status](https://travis-ci.org/vbotka/ansible-freebsd-packages.svg?branch=master)](https://travis-ci.org/vbotka/ansible-freebsd-packages)

[Ansible role.](https://galaxy.ansible.com/vbotka/freebsd_packages/) FreeBSD. Configure repositories. Install and update packages.

Feel free to [share your feedback and report issues](https://github.com/vbotka/ansible-freebsd-packages/issues).

[Contributions are welcome](https://github.com/firstcontributions/first-contributions).


## Requirements

### Collections

- community.general


## Variables

See the defaults and examples in vars.


## Workflow

1) Change shell to /bin/sh

```
shell> ansible host -e 'ansible_shell_type=csh ansible_shell_executable=/bin/csh' -a 'sudo pw usermod user -s /bin/sh'
```

2) Install role and collections

```
shell> ansible-galaxy role install vbotka.freebsd_packages
shell> ansible-galaxy collection install community.general
```

3) Change variables, e.g. in vars/main.yml

```
shell> edit vbotka.freebsd_packages/vars/main.yml
```

See vars/main.yml.sample. See vbotka.freebsd_postinstall/defaults/main/pkgdict_*.yml

4) Create playbook

```
shell> cat freebsd-packages.yml

- hosts: srv.example.com
  roles:
    - vbotka.freebsd_packages
```

5) Manage the packages

Check syntax

```
shell> ansible-playbook freebsd-packages.yml --syntax-check
```

Display variables

```
shell> ansible-playbook freebsd-packages.yml -e pkg_debug=true -t pkg_debug
```

Dry-run the playbook and display changes

```
shell> ansible-playbook freebsd-packages.yml --check --diff
```

Optionally, configure repositories in a separate step. This will enable to display actual dry-run of
the installation.

```
shell> ansible-playbook freebsd-packages.yml -t pkg_conf
```

Dry-run the installation of the packages

```
shell> ansible-playbook freebsd-packages.yml -e pkg_dryrun=true
```

Manage the packages if all seems to be right

```
shell> ansible-playbook freebsd-packages.yml
```


## References

- [FreeBSD handbook: 4.4. Using pkg for Binary Package Management](https://www.freebsd.org/doc/handbook/pkgng-intro.html)
- [FreeBSD handbook: 4.6.2. Configuring pkg Clients to Use a Poudriere Repository](https://www.freebsd.org/doc/handbook/ports-poudriere.html)
- [man pkg.conf](https://www.freebsd.org/cgi/man.cgi?query=pkg.conf&sektion=5)
- [pkg - a binary package manager for FreeBSD](https://github.com/freebsd/pkg#working-with-multiple-repositories)


## Author Information

[Vladimir Botka](https://botka.link)


## License

[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)
