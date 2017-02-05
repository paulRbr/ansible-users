Users - Ansible role
=========

[![Build Status](https://travis-ci.org/paulRbr/ansible-users.svg?branch=master)](https://travis-ci.org/paulRbr/ansible-users)

This role is a very simple machine user management role.

No dependencies and no requirements.

Use this role
-------------

Load this role by adding the following in you `requirements.yml`

    - src: paulrbr.users
      name: users

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: users
           users:
             - name: john
               groups: admin
               key: "{{ lookup('file', 'public_keys/john.pub') }}"


Makefile for easier Ansible calls
------------------

I have written a small Makefile to make your future ansible runs easier. Don't hesitate to [check it out](https://github.com/paulRbr/ansible-makefile/blob/master/Makefile).

Copy it in your ansible configuration directory and start using it via `make help`.


License
-------

GPLv3
