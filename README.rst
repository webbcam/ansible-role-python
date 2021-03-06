Python
======

Ansible role for installing Python from source. Inspired by `this post`_.

Role Variables
--------------

+----------------------+------------------------------+--------------+-------------+
| **Name**             | **Description**              | **Required** | **Default** |
+----------------------+------------------------------+--------------+-------------+
| python_version       | version of python to install | no           | 3.7.2       |
+----------------------+------------------------------+--------------+-------------+
| python_symlink       | set python symlink           | no           | false       |
+----------------------+------------------------------+--------------+-------------+
| python_force_install | force installation of python | no           | false       |
+----------------------+------------------------------+--------------+-------------+


Example Playbook
----------------
::

    - hosts: all
      roles:
         - { role: ansible-role-python, python_version: 2.7.16, python_symlink: yes }

License
-------

BSD

.. _`this post`: https://medium.com/@perwagnernielsen/ansible-tutorial-part-2-installing-packages-41d3ab28337d
