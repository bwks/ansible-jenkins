Role Name
=========

Install Jenkins

Requirements
------------

None

Role Variables
--------------

openjdk_version: Version of open JDK to install defaults to 1.8.0

Dependencies
------------

None

Example Playbook
----------------

- name: Install Jenkins
  hosts: jenkins
  become: True
  roles:
    - { role: ansible-jenkins }

License
-------

GPLv3

Author Information
------------------

Brad Searle
