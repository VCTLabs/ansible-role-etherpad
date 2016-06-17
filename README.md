Role Name
=========

Install Etherpad on RedHat / CentOS 7, Debian Jessie, or Gentoo

Role Variables
--------------

* etherpad_version
* etherpad_topdir
* etherpad_appdir
* admin_user
* admin_password
* nodejs_path
* office_writer_path
* sql_database_type
* sql_database_name
* sql_database_host
* sql_username
* sql_password
* web_server_ip
* web_server_port
* firewall_type
* init_type

Dependencies
------------

No other dependencies.


Example Playbook
----------------

Example playbook

    - hosts: servers
      remote_user: root
      roles:
         - { role: etherpad, sql_username: etherpad, sql_password: password, sql_database_name: etherpad, sql_database_host: localhost, etherpad_version: 3.2.1, firewall_type: firewalld }

License
-------

BSD

Author Information
------------------

S. Lockwood-Childs
