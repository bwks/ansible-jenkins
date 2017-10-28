Role Name
=========

ansible-jenkins

Requirements
------------

Ansible >= 2.2

Role Variables
--------------

```yaml
# Java variables
openjdk_version: Version of open JDK to install defaults to 1.8.0

# Plugins
# This should be a list
jenkins_plugins: 
  - "List of plugin names"

# Web console variables
jenkins_params:
  url_username: "Jenkins URL username - Default: admin"

jenkins_hostname: "Jenkins hostname or IP address - Default: {{ inventory_hostname }}"
jenkins_url_port: "Jenkins URL port - Default: 8080"
jenkins_url_password: "Jenkins URL password"
```

Dependencies
------------

None

Example Playbook
----------------
```yaml
- name: Install Jenkins
  hosts: jenkins
  become: True
  vars_files:
    vars/main.yml
  roles:
    - { role: ansible-jenkins }
```
License
-------

GPLv3

Author Information
------------------

Brad Searle
