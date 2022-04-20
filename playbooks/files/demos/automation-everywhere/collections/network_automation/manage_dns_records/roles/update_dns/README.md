Role Name
=========

network_automation.manage_dns_records.update_dns

Requirements
------------

The following python libraries are required:
- requests

The following collections are required:
- community.general

Role Variables
--------------

Some base information should be defined so your records point to the correct place:
```yaml
subnet: 10.15.120.0/22
vlan: 146
address: 10.15.120.123
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: manage DNS records
  hosts:
    - all
  roles:
    - network_automation.manage_dns_records.update_dns
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>