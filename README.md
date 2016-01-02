redis
=========

A basic standalone Redis install (uses latest stable redis)

Install
-------
Run `ansible-galaxy install NickBall.redis`

Requirements
------------

Requires Ansible 1.9 or higher (may work on lower versions but only tested on 1.9)

Requires internet access to download the specified version of Redis

Role Variables
--------------

No variables are explicity required and use sensible defaults (such as those from the Redis distribution configs)

Most of the configuration options that can be specified in the redis conf are settable as variables. See defaults/main.yml for a full listing

Dependencies
------------

No other dependencies

Example Playbook
----------------

```
    - hosts: redis
      sudo: yes
      roles:
      - NickBall.redis
```

License
-------

MIT

Author Information
------------------

Nick Ball ([Github @nickball](http://github.com/nickball))
