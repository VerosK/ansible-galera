VerosK.galera-cluster
=====================

This is proof of concept role (still working) to setup MariaDB galera role.

Requirements
------------

MariaDB 10.1 is not SELinux-compatible out of the box, so please disable SELinux or tune your policies.

Ansible >= 2.1

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.


Example Playbook
----------------


    - hosts: galera-nodes
      roles:
         - VerosK.galera-cluster

Don't forget to set-up variables

    galera_start_arbiter: False
    galera_start_database: True
    galera_start_master: True
    galera_node_address: "192.168.9.41"

You can also use `mysql_databases`, `mysql_users` 
from `geerlingguy.mysql` role.

License
-------

BSD || WTFPL

Author Information
------------------

Věroš Kaplan

Role sponsored by TeamGuru.com
