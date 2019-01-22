uclalib_role_custom_facts
=========

Ansible role for deploying custom fact script files

Requirements
------------

None.

Role Variables
--------------

* `ansible_root_dir` - defines the root ansible directory - default is `/etc/ansible`

* `ansible_facts_dir` - defines the directory to store the custom fact script files - default is `/etc/ansible/facts.d`

* `ansible_facts_file_pattern` - defines the file pattern to use when searching for custom fact script files to deploy to all OS distributions - default is `*_custom.fact`

* `ansible_facts_rhel_file_pattern` - defines the file pattern to use when searching for custom fact script files to deploy to RHEL distributions - default is `*_rhel.fact`

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- name: uclalib_customfacts.yml
  become: yes
  become_method: sudo
  hosts: all

  roles:
    - { role: uclalib_role_custom_facts }
```
