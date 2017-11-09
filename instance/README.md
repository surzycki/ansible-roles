Role Name: Instance
=========

Provision an ec2 instance

Requirements
------------

boto

Role Variables
--------------

```yaml
instances:
  - name: frontend servers
    env: production
    type: t2.small
    count: 1
    group: frontend
    security_groups:
      - ssh
      - http
    monitoring: yes

base_image: ami-f95ef58a
```

The group is the server group the server belongs to

Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: infrastructure
      roles:
         - instance

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
