Elixir
========

An ansible role that install Erlang/OTP & Elixir.

Requirements
------------

Tested on Ansible 2.2.0

sudo to run.

Role Variables
--------------

```
- elixir_version: elixir version (v1.1.1, v1.1.0, v1.0.5, ...)
- erlang_version: erlang version (18.1, 18.0, 17.5, ...)
```

Dependencies
------------

none

Example Playbook
----------------

```
- hosts: servers
  sudo: yes
  roles:
     - { role: elixir, erlang_version: 18.2, elixir_version: v1.3.2, erl_configure_options: '--enable-hipe --enable-smp-support' }
```

License
-------

MIT

Author Information
------------------

Sergey Gernyak
ohr486 (actually a big part of code is taken from this [repo](https://github.com/ohr486/ansible-elixir))
