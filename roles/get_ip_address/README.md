Role Name
=========

jjaswanson4.jdc.get_ip_address

Requirements
------------

The following python libraries are required:
- pynetbox

The following collections are required:
- netbox.netbox

Role Variables
--------------

N/A, although credentials are required:

```yaml
netbox_url: netbox.domain.lcl
netbox_username: netbox-admin
netbox_password: 'su3prs3c4r3'
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: get IP address
  hosts:
    - all
  roles:
    - jjaswanson4.jdc.get_ip_address
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>