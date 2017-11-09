Role Name
=========

Gets facts for groups, facts returned will be in the format:

* ec2_frontend_instances
* ec2_api_instances
* ec2_staging_instances
* etc

Requirements
------------

Running instances

Role Variables
--------------


Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      roles:
        - { role: instance-facts, tags: [ 'instance-facts'] }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
