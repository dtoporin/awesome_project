network_management
=========

Ansible role for changing a name of an active network interface

Requirements
------------

There are no specific requirements

Role Variables
--------------

Variables that are in defaults/main.yml
| Variable | default value |
| ------------- | ------------- |
| network.interface.name  | "net0"  |


Example Playbook
----------------

    - hosts: servers
      roles:
         - network_management

License
-------

MIT
