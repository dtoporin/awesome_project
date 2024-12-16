disk_encryption
=========

Ansible role for encrypting the partition in the system (partition name should be specified in the inventory).
>[!CAUTION]
>This role has destructive tasks. 
>Passphrase in role used in plaintext for testing and educational purposes. Don't use this way in production environment.

Requirements
------------

There are no specific requirements

Role Variables
--------------

Variables that are in defaults/main.yml
| Variable  | default value |
| ------------- | ------------- |
| luks.target_disk  | "" |
| luks.passphrase  | "cryptoCrypt" |
| luks.name  | "cryptoName" |
| luks.label  | "cryptoLabel" |

Example Playbook
----------------

    - hosts: servers
      roles:
         - partition_encryption

License
-------

MIT
