=========================================
vbotka.freebsd_packages 2.7 Release Notes
=========================================

.. contents:: Topics


2.7.4
=====

Release Summary
---------------
Update repo configuration.

Major Changes
-------------

Minor Changes
-------------
* Update tasks conf.yml
* Add template repos.j2

Bugfixes
--------
* Fix template repo.j2

2.7.3
=====

Release Summary
---------------
Update contrib/pkgdict_*; Support 14.3

Major Changes
-------------

Minor Changes
-------------
* Update contrib/pkgdict_*
* Update meta; Support 14.3
* Update README.


2.7.2
=====

Release Summary
---------------
Maintenace update.

Major Changes
-------------

Minor Changes
-------------
* Update README. Fix link.


2.7.1
=====

Release Summary
---------------
Maintenace update.

Major Changes
-------------

Minor Changes
-------------
* Update README.
* Updated contrib/vars/pkgdict_*.yml


2.7.0
=====

Release Summary
---------------

Major Changes
-------------
* Support 13.4, 13.5, 14.1, and 14.2
* Bump Ansible version to 2.18

Minor Changes
-------------
* Improved formatting
* Sanity assert set quiet=true
* Optionally delegate pkgng to vmm host
* Add variable pkg_delegate (default='')
* Add sanity test pkg_jail is required when pkg_delegate not empty.

Bugfixes
--------

Breaking Changes / Porting Guide
--------------------------------
