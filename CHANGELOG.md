# Ansible Role for PHP

## 2.1.0 - TBC

### Major Changes

  - Install composer globally with official installer (<https://getcomposer.org/installer>)
  - Install more dev tools with cgr
  - CI with ansible-lint and galaxy-lint-rules
  - Create `/etc/profile.d/composer.sh` with templates
  - Source environment variables with `su -l -s /bin/bash -c`
  - Use shell only when shell functionality is required
  - Replace tests from Docker to LXD
  - Reduce kernel logging level during CI

## 2.0.0 - 2018-10-25

  - Ininitial release for Ansible 2.6
  - Support both Ubuntu 16.04/18.04 or RHEL/CentOS 6/7
  - Install PHP 5.6 on Ubuntu 16.04 from PPA
  - Install PHP 7.2 on Ubuntu 18.04 from PPA
  - Install PHP 5.6 on CentOS 6 from IUS
  - Install PHP 7.2 on CentOS 7 from IUS
