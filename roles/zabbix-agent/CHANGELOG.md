#kalloa zabbix-agent changes:

0.0.1	(2016-06-16)
  * Removed external modules(zabbix_host and zabbix_hostmacro) because its already integrated in Ansible.
  * Some changes for our repo compatibility

#gunkiniu zabbix-agent changes:

Below an overview of all changes

Version (Release date)

0.6.1   (2016-05-27)
  * Add Suse, Solaris
  * zabbix_agentd.conf name into vars
  * add http(s)_proxy for installing pkgs

0.6.0   (2016-05-12)

  * Changed sudo to become. #30 (By pull request: UnderGreen (Thanks!))
  * No reason for zabbix to able to change its own config #25 (By pull request: burner1024 (Thanks!))
  * Updated documentation for Zabbix 3.0
  * Updated Zabbix 3.0 OS list
  * Fixed tests

0.5.0   (2016-02-16)

  * Zabbix 3.0
  * Moved "set_facts" to var files.
  * Added basic travis-si test.

0.4.0   (2016-01-31)

  * zabbix_host_groups not working as expected #4 (By pull request: Pion (Thanks!))
  * set cache_valid_time=0 to ensure an apt-get update after the added repo-key (By pull request: lhoss (Thanks!))
  * Add api tag to set_fact. Fixes #19 (By pull request: kostyrevaa (Thanks!))
  * add sudo, and add zabbix-api dependency to readme.md (By pull request: Savemech (Thanks!))
  * default zabbix_agent to all interfaces #14 (By pull request: dlbewley (Thanks!))
  * enable use of EPEL packages #11 (By pull request: dlbewley (Thanks!))
  * Fixed kitchen test setup
  * Removed zabbix_group (is already in Ansible), updated zabbix_host
  * Added tag: zabbix-agent

0.3.0   (2015-08-25)

  * Fixes for RHEL 6 Server on ansible 1.9.2 #10 (By pull request: bwaters (Thanks!))
  * remove macros from defaults fixes issue #7 (By pull request: kostyrevaa (Thanks!))
  * defaults/main.yml is not in line with the README #5 (By pull request: dhxgit (Thanks!))
  * Added empty dependencies list to meta/main.yml #3 (By pull request: neneko-mun (Thanks!))
  * Ubuntu is uppercase in ansible_distribution #2 (By pull request: wascheck (Thanks!))

0.2.1   (2015-03-20)

  * Create hostgroups requires zabbix_api #1 (By pull request: wascheck (Thanks!))

0.2.0   (2015-03-06)

  * Added some "cove" modules for automatically creating agents in webinterface via api
  * Updated template for correct listeninterface

0.1.0   (2015-02-01)

  * Updated readme; added double quotes on names; added var zabbix_repo;

0.0.2   (2014-11-05)

  * Added suse as operating system
  * Updated documentation
  * Updated the name for the debian repositories for including deb or deb-src


0.0.1   (2014-11-01)

  * Initial Version
