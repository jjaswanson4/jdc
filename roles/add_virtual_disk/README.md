Role Name
=========

jjaswanson4.jdc.add_virtual_disk

Requirements
------------

Depending on the task file used, certain python libraries are required:
- pyVmomi
- aiohttp

Role Variables
--------------

Define the following to have the role add storage:
```yaml
additional_storage:
  - size: 600Gb
    type: thin
    scsi_controller: 0
    unit_number: 1
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: manage storage
  hosts:
    - all
  roles:
    - jjaswanson4.jdc.add_virtual_disk
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>