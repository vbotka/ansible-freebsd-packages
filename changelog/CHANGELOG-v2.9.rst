=========================================
vbotka.freebsd_packages 2.9 Release Notes
=========================================

.. contents:: Topics


2.9.3
=====

Release Summary
---------------

Major Changes
-------------

Minor Changes
-------------
* Move .ansible-lint.local to .ansible-lint; Galaxy does not use
  .ansible-lint from a role.


2.9.2
=====

Release Summary
---------------
Add optional UCL configuration by vbotka.freebsd.ucl

Major Changes
-------------

Minor Changes
-------------
* Update meta: Require collection vbotka.freebsd
* Add variable: pkg_repos_conf_ucl (default=[])
* Update defaults and vars samples.
* Fix task: Remove repos not listed in pkg_repos_conf


2.9.1
=====

Release Summary
---------------
Added an option to fetch packages into the local repository.

Major Changes
-------------

Minor Changes
-------------
* Add handler to generate repo metadata.
* Update debug task.
* Update tasks formatting.
* Add variables defaults
  pkg_fetch=false
  pkg_fetch_dir=/usr/local/repo
  pkg_fetch_dir_owner=root
  pkg_fetch_dir_group=wheel
  pkg_fetch_dir_mode='0755'


2.9.0
=====

Release Summary
---------------
Ansible 2.21 upgrade.

Major Changes
-------------
* Supported 14.4, 15.0, and 15.1

Minor Changes
-------------

Bugfixes
--------

Breaking Changes / Porting Guide
--------------------------------
