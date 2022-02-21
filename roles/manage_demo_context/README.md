Role Name
=========

jjaswanson4.jdc.manage_demo_context

Requirements
------------

The following python libraries are required:
- pynetbox
- pyVmomi
- requests

The following collections are required:
- netbox.netbox
- redhat.satellite
- community.vmware

Role Variables
--------------

The intention of this role is to set up a "context" to contain a demo, such as:
- dns zone
- vcenter folder
- dns zone in satellite (for provisioning)
- netbox tenant

A few vars are needed:
```yaml
base_dns_suffix: demos.lcl
demo_uuid: 1234
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: manage demo context
  hosts:
    - all
  roles:
    - jjaswanson4.jdc.manage_demo_context
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>
