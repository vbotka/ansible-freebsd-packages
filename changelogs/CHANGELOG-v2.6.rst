=========================================
vbotka.freebsd_packages 2.6 Release Notes
=========================================

.. contents:: Topics


2.6.4
=====

Release Summary
---------------
Maintenance update.

Major Changes
-------------

Minor Changes
-------------
* Labels formatting.
* Update debug. Redundant vars removed.
* Update pkg_repos_conf examples in defaults/main.yml

2.6.3
=====

Release Summary
---------------
Feature update.

Major Changes
-------------
* Enable upgrade (state=latest) in the form “category/port”, or
  “pkg-origin
* Update tasks/main.yml, pkg_delete.yml,  and pkg_install.yml

Minor Changes
-------------
* Update README


2.6.2
=====

Release Summary
---------------
Feature update.

Major Changes
-------------
* Add sanity.yml various checks.
* Add var pkg_sanity default=true.
* Add var pkg_sanity_version_community_general default=true.
* Add var pkg_version_community_general requirement minimal 9.3.0
* Update debug.yml
* Rename packages_*.yml to pkg_*.yml
* Rename tags: pkg_delete, pkg_install

Minor Changes
-------------
* Update README


2.6.1
=====

Release Summary
---------------
Ansible 2.17 update

Major Changes
-------------
* Add supported 14.1
* Update and fix lint.

Minor Changes
-------------
* Update README
* Update debug
* Add pkg_backup_conf to debug output.
* Add var pkg_role_version


2.6.0
=====

Release Summary
---------------
Ansible 2.16 update

Major Changes
-------------
* Supported FreeBSD 13.3 and 14.0

Minor Changes
-------------
* Update ansible lint config.
* Update README.
* Fix Ansible lint.
* Add contrib/vars/pkgdict_*.yml

Bugfixes
--------

Breaking Changes / Porting Guide
--------------------------------
