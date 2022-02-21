Role Name
=========

jjaswanson4.jdc.manage_systems_with_satellite

Requirements
------------

The following python libraries are required:
- pynetbox
- requests

The following collections are required:
- netbox.netbox
- redhat.satellite

Role Variables
--------------

Define the vars needed to provision a system via Red Hat Satellite:

```yaml
provisioning:
  cpus: 4
  memory_mb: 16384
  host_group: rhel8
  organization: org1
  location: loc1
  method: bootdisk
  dns_domain: domain.lcl
  activation_keys: ak-rhel8
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: provision systems via Satellite
  hosts:
    - all
  roles:
    - jjaswanson4.jdc.manage_systems_with_satellite
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>