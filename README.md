# Ansible role: mysql
Installs and configures MariaDB.

## Requirements
+ ansible > 2.2.0

## Role Variables
|Key|Type|Description|Default|
|:--|:---|:----------|:------|
|mysql_version|String||10.1|
|mysql_enablerepo|String||mariadb|
|mysql_packages|Array||See `defaults/main.yml`|
|mysql_log_dir|String||/var/log/mysql|
|mysql_user_home|String||/root|
|mysql_root_username|String||root|
|mysql_root_password|String||password|

## Dependencies
None.

## Example playbook

```yaml
- hosts: all
  roles:
    - { role: mysql }
  vars:

```
