Role Name
=========

jjaswanson4.jdc.manage_dns_records

Requirements
------------

The following python libraries are required:
- pynetbox

The following collections are required:
- netbox.netbox
- community.general

Role Variables
--------------

No vars are needed as the role pulls the assigned IP address from netbox then puts it into IDM

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: manage dns records
  hosts:
    - all
  roles:
    - jjaswanson4.jdc.manage_dns_records
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>