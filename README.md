Role Name
=========

Installs a new medusa development KVM/libvirt virtual host following
an initial system load, which has been snapshotted as `Snapshot 1`, if
used with the playbook supplied in the root of the role.

Requirements
------------

- Access to the medusa staging server to obtain a mongodb dump to be
  placed under the file directory of the role as `trmn.tar.gz`.
- A encrypted password stored under `credentials/medusa-medusa-password`.
  (This file can be created using `openssl passwd -6` and capturing
  the output to that file.)

Role Variables
--------------
See `defaults/main.yml` and `vars/*` (particularly `vars/nginx-vars.yml`).

Dependencies
------------

- geerlingguy.git
- geerlingguy.composer
- geerlingguy.nginx
- geerlingguy.nodejs
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