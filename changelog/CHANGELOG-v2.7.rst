=========================================
vbotka.freebsd_packages 2.7 Release Notes
=========================================

.. contents:: Topics


2.7.1
=====

Release Summary
---------------
Maintenace update.

Major Changes
-------------

Minor Changes
-------------


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
