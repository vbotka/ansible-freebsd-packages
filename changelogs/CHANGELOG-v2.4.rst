=========================================
vbotka.freebsd_packages 2.4 Release Notes
=========================================

.. contents:: Topics


2.4.1
=====

Release Summary
---------------
Add tasks stat.yml. Optionally create dictionary of vulnerabilities
pkg_audit.

Minor Changes
-------------
- Add variables: pkg_stat, pkg_audit_enable (default=false)

2.4.0
=====

Release Summary
---------------
Simplified configuration of repositories. Single unified template
repo.j2 for repositories. Simplified configuration of optional
parameters of *community.general.pkgng*

Major Changes
-------------
- Split tasks: packages_install.yml and packages_delete.yml
- community.general.pkgng; Optional parameters moded to *module_defaults*
- Assert *pkg_state*
- Simplified loop arguments in packages_*.yml
- Simplified set_fact: pkg_*
- Add support for all parameters of community.general.pkgng
- Add variables: pkg_default_repo_template, pkg_repos_template
  (default repo.j2)
- Add tags: pkg_packages_install_*, 
- README; Add examples.
- vars/main.yml.sample; Add examples.

Minor Changes
-------------
- Debug formatting

Breaking Changes / Porting Guide
--------------------------------
- Default pkg_install_individually changed to false
- Defaults changed for pkg_default_repo_*
- Rename variable *pkg_repo* to *pkg_repos_conf*
- Removed templates: FreeBSD.conf.j2, FreeBSD.conf.full.j2
- Updated defaults
