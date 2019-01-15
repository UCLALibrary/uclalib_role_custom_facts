uclalib_role_custom_facts
=========

Ansible role for deploying custom fact files

Requirements
------------

None.

Role Variables
--------------

* `variable` - defines the version of FITS to download/install on the system

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
