Role Name
=========

security_automation.os.rhel

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
- name: Enforce security baseline on RHEL
  hosts:
    - all
  roles:
    - security_automation.os.rhel
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>