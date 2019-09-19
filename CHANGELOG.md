# Ansible Role for PHP

## 3.5.0 - TBC

### Major Changes

  - Default with Python 3

## 3.4.0 - 2019-09-18

### Major Changes

  - Run molecule test manually on Travis CI
  - Abstract package parameters with multiple version support
  - Install both php-cli and php-fpm

## 3.3.0 - 2019-08-27

### Major Changes

  - Update for RHEL 7
  - Add Vagrant test for RHEL 7

## 3.2.0 - 2019-07-08

### Major Changes

  - Update LXD test profile for Kubernetes v1.15.0 support
  - Fix molecule `group_vars` with links
  - Replace `with_items` with `loop`
  - Replace `with_dict` with `var`
  - Replace `with_first_found` with `lookup('first_found')`

## 3.1.0 - 2019-06-13

### Major Changes

  - Always include default variables from `vars/main.yml`
  - Always use `become: true` with molecule, especially for vagrant
  - Simplify for openSUSE by `disable_gpg_check: true`

## 3.0.0 - 2019-05-20

### Major Changes

  - Upgrade minimal Ansible support to 2.8.0

## 2.6.0 - 2019-05-04

### Major Changes

  - Refine Travis CI Molecue test cases

## 2.5.0 - 2019-04-17

### Major Changes

  - Run test with `travis_wait 120`

## 2.4.0 - 2019-03-03

### Major Changes

  - Unify variable name as `repository` and `package`
  - Add openSUSE Leap 15 support
  - Remove CentOS 6 support

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
