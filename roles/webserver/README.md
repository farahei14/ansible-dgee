Role Name
=========

Installation serveur web Apache

Requirements
------------

- CentOS 6.6
- Epel repository (for phpMyAdmin)

Role Variables
--------------

- admin_email: set admin email in apache configuration (default: root@localhost)
- webserver_port: set apache default listening port (default: 80)
- a2_script_directory: where do you want to copy a2ensite and a2dissite script (default: /usr/bin)
- install_phpmyadmin: install package phpmyadmin (yes|no) (default: no)

Dependencies
------------

No dependencies

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: webserver, tags: ['webserver_install']  }

License
-------

GPLv2

Author Information
------------------

James HORLEY

