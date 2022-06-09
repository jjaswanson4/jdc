Role Name
=========

virtualization_automation.manage_systems.provision_system

Requirements
------------

The following python libraries are required:
- requests

The following collections are required:
- community.general
- community.vmware

Role Variables
--------------

Some base information should be defined, otherwise sane defaults will be used:
```yaml
subnet: 10.15.120.0/22
vlan: 146
address: 10.15.120.123
cpus: 4
memory_mb: 16384
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: provision a system
  hosts:
    - all
  roles:
    - virtualization_automation.manage_systems.provision_system
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>