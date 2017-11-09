Role Name: Security Group
=========

Setups up security groups on EC2

Requirements
------------

boto

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```yaml
security-groups:
  - name: http
    description: http/https traffic
    rules:
      - proto: tcp
        from_port: 80
        to_port: 80
        cidr_ip: 0.0.0.0/0
      - proto: tcp
        from_port: 443
        to_port: 443
        group_id: amazon-elb/sg-87654321/amazon-elb-sg

```

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      connection: local
      gather_facts: False
      roles:
         - security-group

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
