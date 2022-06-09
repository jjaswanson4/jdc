Role Name
=========

os_automation.rhel.soe

Requirements
------------

The following python libraries are required:
- N/A

The following collections are required:
- N/A

Role Variables
--------------

No base information is required, simply point the role at a RHEL system.
```yaml
all:
  children:
    rhel:
      system-1.whatever.lcl:
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: enforce SOE on RHEL
  hosts:
    - all
  roles:
    - os_automation.rhel.soe
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>