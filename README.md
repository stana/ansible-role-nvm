Role Name
=========

NVM and nodejs (optional) installation role.

Role Variables
--------------

defaults/main.yml - nvm_ver, nvm_dir, node_ver (optional).

By default only nvm will be installed. To install nodejs also set node_ver.

Dependencies
------------

None.

Example Playbook
----------------

To only install nvm.

    - hosts: servers
      roles:
         - { role: stana.nvm, nvm_ver: 0.32.1 }

To install nvm and nodejs set node_ver.

    - hosts: servers
      roles:
         - { role: stana.nvm, nvm_ver: 0.32.1, node_ver: 6.7 }

License
-------

MIT
