# Ansible Role for PHP

## 2.4.0 - TBC

### Major Changes

## 2.3.0 - 2019-01-30

### Major Changes

  - Porting test to Molecule based

## 2.2.0 - 2019-01-26

### Major Changes

  - Improve variables default value handling

### CentOS

  - Enable IUS manually

## 2.1.0 - 2018-12-06

### Major Changes

  - CI with yamllint, ansible-lint and ansible-playbook --syntax-check
  - CI with LXD, improve systemd support
  - Use shell only when shell functionality is required
  - Install composer globally with official installer (<https://getcomposer.org/installer>)
  - Template `/etc/profile.d/composer.sh` for environment variables
  - Source environment variables with `su -l -s /bin/bash -c`
  - Default install PHP 5.6 on Ubuntu 16.04 and CentOS 6
  - Default install PHP 7.2 on Ubuntu 18.04 and CentOS 7
  - Support override with defaults/main.yml

### CentOS

  - Don't install epel-release, conflict with RHEL
  - Don't install ius-release, assume yum already handle it

## 2.0.0 - 2018-10-25

  - Ininitial release for Ansible 2.6
  - Support both Ubuntu 16.04/18.04 or RHEL/CentOS 6/7
  - Install PHP 5.6 on Ubuntu 16.04 from PPA
  - Install PHP 7.2 on Ubuntu 18.04 from PPA
  - Install PHP 5.6 on CentOS 6 from IUS
  - Install PHP 7.2 on CentOS 7 from IUS
