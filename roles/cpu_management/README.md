cpu_management
=========

Ansible role for changing a name of an active network interface
    - Disabling C-state for all available CPUs.
    - Switching CPU operation from power-saving mode to more productive mode.

Requirements
------------

There are no specific requirements

Role Variables
--------------

Variables that are in defaults/main.yml
| Variable | default value |
| ------------- | ------------- |
| cpu_governor_mode | "performance"  |


Example Playbook
----------------

    - hosts: servers
      roles:
         - cpu_management

>[!IMPORTANT]
>Manual reboot needed for applying changes or you can use 'ansible.builtin.reboot' module to reboot automatically
>Or use ansible handler `Restart host` in playbook, but need to set var `allow_reboot` to `true` value

License
-------

MIT
