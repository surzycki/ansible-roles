Role Name: Puma
=========

Installs puma as an upstart service

Requirements
------------

Ruby

Role Variables
--------------

```yaml
puma:
  - service: api
    root: /var/www/api/current
    config: /var/www/api/shared/config/puma.rb
```

Dependencies
------------

Ruby

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: puma, tags: [ 'puma'] }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
