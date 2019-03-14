Python
======

Ansible role for installing Python from source.

Role Variables
--------------

+----------------------+------------------------------+----------+---------+
| name                 | description                  | required | default |
+----------------------+------------------------------+----------+---------+
| python_version       | version of python to install | no       | 3.7.2   |
+----------------------+------------------------------+----------+---------+
| python_symlink       | set python symlink           | no       | false   |
+----------------------+------------------------------+----------+---------+
| python_force_install | force installation of python | no       | false   |
+----------------------+------------------------------+----------+---------+


Example Playbook
----------------

    - hosts: all
      roles:
         - { role: webbcam.python, python_version: 2.7.16, python_symlink: yes }

License
-------

BSD
