Ansible Role: cpu-stats
=========
[![CI](https://github.com/nmishin/cpu-stats-ansible/workflows/CI/badge.svg?event=push)](https://github.com/nmishin/cpu-stats-ansible/actions?query=workflow%3ACI)

An Ansible Role that installs [cpu-stats](https://github.com/Nmishin/cpu-stats) on Linux.

Requirements
------------
None.

Role Variables
--------------
Available variables are listed below, along with default values (see defaults/main.yml):

    app_version: '0.9.0'
    base_path: '/opt/nmishin/cpu-stats'

Version of app can be found in the app repo: https://github.com/Nmishin/cpu-stats

Dependencies
------------
None.

Example Playbook
---------------

    - hosts: myservers
      become: yes
      become_user: root
      roles:
        - cpu-stats-ansible

License
-------

BSD

Author Information
------------------
This role was created in 2023 by [Nikolai Mishin](https://www.linkedin.com/in/nikolai-mishin/)
