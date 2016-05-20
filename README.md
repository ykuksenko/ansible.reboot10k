reboot10k
=========

Simple reboot role.

Name is a inspired by the r10k ruby gem, which is a great, unrelated, idea.

Requirements
------------

None.

Role Variables
--------------

     #optional ssh port to watch to reliably tell if the host rebooted
     #default: 22
     reboot10k_watch_port: 44

Dependencies
------------

None

Example Playbook
----------------

You can specify a port to watch:

    - hosts: servers
      roles:
         - { role: reboot10k, reboot10k_watch_port: 44 }

But you don't have to:

    - hosts: servers
      roles:
         - reboot10k

License
-------

GPLv3

Author Information
------------------

Jesse Lang - said to put it on Ansible Galaxy.

Lloyd Benson - added the reboot delay. also needed to reboot a computer.

Yevgeniy Kuksenko - needed to reboot a computer. got to name the role.
