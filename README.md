Ansible Role: cpu-stats
=========
[![CI](https://github.com/Nmishin/cpu-stats-ansible/actions/workflows/ci.yml/badge.svg)](https://github.com/Nmishin/cpu-stats-ansible/actions/workflows/ci.yml)

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

You can choose any base_path, but according to FHS, we need to install packages to the /opt/'provider'/'package'

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
