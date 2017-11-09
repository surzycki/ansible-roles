Role Name: Memcached
=========

Install and configure memcached

Requirements
------------

None

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```yaml
memcached_port: 11211
memcached_listen_address: 0.0.0.0
memcached_max_conn: 1024
memcached_cache_size: 64
memcached_fs_file_max: 756024
```


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  roles:
     - memcached
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
