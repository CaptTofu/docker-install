Docker Install 
=========

Install Docker

Requirements
------------

In a private cloud you need to have a VM deployed with a user having sudo permission and SSH key authentication.

Role Variables
--------------

remote_user : The user on the docker host having SSH authentication and sudo permission
target      : The docker host


Dependencies
------------

None

Example Playbook
----------------

- hosts: "{{ target | default('servers') }}"
  sudo: true
  roles:
  - docker-install

License
-------

Apache 2.0

Author Information
------------------

Patrick Galbraith
Michael Scheetz
