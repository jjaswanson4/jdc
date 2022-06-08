Role Name
=========

jjaswanson4.jdc.manage_cmdb_records

Requirements
------------

The following python libraries are required:
- pynetbox

The following collections are required:
- netbox.netbox

Role Variables
--------------

Some base information should be defined for when the role creates a record in netbox:
```yaml
cpus: 4
memory_mb: 16384
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: manage CMDB records
  hosts:
    - all
  roles:
    - cmdb_automation.manage_records.manage_instance_records
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>