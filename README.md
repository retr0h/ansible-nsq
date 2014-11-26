nsq
===

A role which installs and manages NSQ.

Role ready status
-----------------

[![Build Status](http://img.shields.io/travis/retr0h/ansible-nsq.svg?style=flat-square)](https://travis-ci.org/retr0h/ansible-nsq)
[![Galaxy](http://img.shields.io/badge/galaxy-ansible--nsq-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/2265)

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml

Dependencies
------------

None

Example Playbook
----------------

Install nsqadmin on given set of nodes:

    - hosts: nsqadmin
      roles:
        - { role: nsq, nsq_nsqadmin_server: true }

Install nsqd on given set of nodes:

    - hosts: nsq
      roles:
        - { role: nsq, nsq_nsqd_server: true }

Install nsqlookupd on given set of nodes:

    - hosts: nsqlookupd
      roles:
        - { role: nsq, nsq_nsqlookupd_server: true }

License
-------

MIT
