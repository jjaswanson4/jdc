Role Name
=========

jjaswanson4.jdc.install_aap

Requirements
------------

The initial install files for AAP should be available for the role to pull

Role Variables
--------------

Define the following to have the role add storage:
```yaml
aap_download_url: http://webserver.domain.lcl/ansible-automation-platform-setup-2.1.0-1.tar.gz
aap_bundle: ansible-automation-platform-setup-2.1.0-1.tar.gz
controller_install:
  admin_password: admin
  pg:
    password: password123
bootstrap_controller: yes
```

Dependencies
------------

N/A

Example Playbook
----------------

```yaml
- name: install AAP
  hosts:
    - all
  roles:
    - jjaswanson4.jdc.install_aap
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>