<a href="https://www.bitbull.ch"><img src="https://www.bitbull.ch/wiki/images/teamwork-trans.png" alt="Bitbull" width="250px"/></a>

# joe-speedboat.mariadb
This Ansible Role installs & configures mariadb, as well as manages content (db & user).

## Installation with ansible-galaxy:
```bash
ansible-galaxy install joe-speedboat.mariadb
```

## Install with git:
```bash
git clone https://github.com/joe-speedboat/ansible.mariadb.git /etc/ansible/roles/joe-speedboat.mariadb
```

## Requirements
* Tested with Ansible 13.2.0 
* OS Releases:
  * Rocky9

## Role dependencies
This Ansilbe Role has no dependencies to other Ansilbe Roles

## Collection depencies

* community.mysql
```bash
ansible-galaxy collection install -r collections/requirements.yml
```

## Role Variables
Variables are self speaking or documented in:   
* `defaults/main.yml`
* `vars/main.yml`

The following variables can be overridden:
 * `mariadb_secure_installation`: Default: false. Similar to `mysql_secure_installation`
 * `mariadb_root_password`: Default: ''.
 * `mariadb_databases`: Default: {} . Dictionary with databases.
 * `mariadb_users_create`: Default: {}. Dictionary with user credentials.
 * `mariadb_users_remove`: Default: {}. Dictionary of users to remove.

## Example Playbook
Example playbooks for this role are located in ´test´ folder:
* `test/playbook_mariadb_minimal.yml`: Minimal role for testing
* `test/playbook_mariadb.yml`: Real life example
* `test/playbook_mariadb_full.yml`: Full example with all possible vars.  

## License
https://opensource.org/licenses/LGPL-3.0    
Copyright (c) Chris Ruettimann <chris@bitbull.ch>

