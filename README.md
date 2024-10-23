Role Name
=========

Installs a new medusa development host following an initial system load.

Requirements
------------

Access to the medusa staging server.

Role Variables
--------------



Dependencies
------------

- geerlingguy.git
- geerlingguy.php
- geerlingguy.php-versions
- geerlingguy.repo-epel
- geerlingguy.repo-remi
- nginxinc.nginx


Example Playbook
----------------

    - hosts: medusa-dev-server
      roles:
         - doug-needham.medusa

License
-------

BSD-3

Author Information
------------------

This role was created in 2024 by [Doug Needham](https://www.ka8zrt.com)