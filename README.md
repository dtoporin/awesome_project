Usefull playbook for setup servers
=========
This playbook play three roles
    - network_management
    - disk_encryption
    - cpu_management

>[!CAUTION] 
>This playbook included roles with destructive tasks.
>Passphrase in role used in plaintext for testing and educational purposes. Don't use this way in production environment.

Requirements
------------

There are no specific requirements

Role Features
--------------

All vars in playbook described in roles README files
Specific var in playbooks `allow_reboot: [true|false]` needed for allow or disallow host reboot to applying new confgiuration

Also playbook has a task for getting CPU info

License
-------

MIT
