Role Name: Redis
=========

Install and configure redis

Requirements
------------

None

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```yaml
edis_port: 6379
redis_bind_interface: 127.0.0.1
redis_unixsocket: ''
redis_timeout: 300

redis_loglevel: "notice"
redis_logfile: /var/log/redis/redis-server.log

redis_databases: 16

# Set to an empty set to disable persistence (saving the DB to disk).
redis_save:
  - 900 1
  - 300 10
  - 60 10000

redis_rdbcompression: "yes"
redis_dbfilename: dump.rdb
redis_dbdir: /var/lib/redis

redis_maxmemory: 0
redis_maxmemory_policy: "noeviction"
redis_maxmemory_samples: 5

redis_appendonly: "no"
redis_appendfsync: "everysec"

# Add extra include files for local configuration/overrides.
redis_includes: []
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
     - redis
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
