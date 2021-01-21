
MariaDB Setup with Ansible
=================

* install and configure MariaDB

Requirements
------------

* Currently tested with CentOS 7 and 8
* Ansible 2.4 or higher is required for this Ansible Role

Role Variables
--------------
Variables are self speaking or documented in:   
* `defaults/main.yml`
* `vars/main.yml`

The following variables can be overridden:
 * `mariadb_secure_installation`: Default: false. Similar to `mysql_secure_installation`
 * `mariadb_root_password`: Default: ''.
 * `mariadb_databases`: Default: {} . Dictionary with databases.
 * `mariadb_users_create`: Default: {}. Dictionary with user credentials.
 * `mariadb_users_remove`: Default: {}. Dictionary of users to remove.

Dependencies
------------

This Ansilbe Role has no dependencies to other Ansilbe Roles

Example Playbook
----------------

Example playbooks for this role are located in ´test´ folder:
* `test/playbook_mariadb_minimal.yml`: Minimal role for testing
* `test/playbook_mariadb.yml`: Real life example
* `test/playbook_mariadb_full.yml`: Full example with all possible vars.  

License
--------------
https://opensource.org/licenses/LGPL-3.0    
Copyright (c) Chris Ruettimann <chris@bitbull.ch>
