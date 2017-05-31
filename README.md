Clarivate-LSPS.promdash
=======================

Installation for [Prometheus Dashboard](https://github.com/prometheus-junkyard/promdash)

Role Variables
--------------

### Mandatory variables

None.

### Optional variables

```yaml
# gosu util version. Used with init.d service mode
gosu_version:   '1.10'

# User and group
promdash_user:   promdash
promdash_group:  promdash

# Paths
promdash_install_path:  /opt/promdash
promdash_log_path:      /var/log/promdash
promdash_pid_path:      /var/run/promdash
promdash_data_dir:      /var/lib/promdash/data

promdash_port: 9060
```


Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
         - { role: Clarivate-LSPS.promdash }

License
-------

MIT
