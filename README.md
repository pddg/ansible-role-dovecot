Role Name
=========

Role for install and configure Dovecot.

Requirements
------------

You should have `sudo` permission. And this role require certificates. Let's encrypt is very useful for this.

Role Variables
--------------

See [defaults/main.yml](./defaults/main.yml)

Dependencies
------------

No dependencies

Example Playbook
----------------

```yaml
- hosts: all
  become: yes
  roles:
    - name: pddg.dovecot
      var:
        dovecot_ssl_options:
          cert: /path/to/cert
          key: /path/to/key
```

License
-------

MIT

Author Information
------------------

[pddg](https://github.com/pddg/)
  - Web: [poyo.info](https://www.poyo.info/)

