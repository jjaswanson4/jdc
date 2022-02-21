Role Name
=========

jjaswanson4.jdc.common_config

Requirements
------------

This collection is built on top of various collections, such as:
- redhat.rhel_system_roles
- linux-system-roles

Role Variables
--------------

Check the upstream roles/collections for full details, but a few vars are:
```yaml
config_files:
  - hosts
  - resolv.conf
timesync_ntp_servers:
  - hostname: 0.rhel.pool.ntp.org
    iburst: yes
  - hostname: 1.rhel.pool.ntp.org
    iburst: yes
  - hostname: 2.rhel.pool.ntp.org
    iburst: yes
  - hostname: 3.rhel.pool.ntp.org
    iburst: yes
selinux_policy: targeted
selinux_state: permissive
dns_resolv:
  search_domains:
    - lab.msp.redhat.com
  nameservers:
    - 8.8.8.8
    - 8.8.4.4
  options:
    - 'timeout:1'
base_packages:
  disable_gpg_check: yes
  packages:
    - lsof
    - vim
    - sos
    - redhat-support-tool
    - open-vm-tools
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
    - jjaswanson4.jdc.common_config
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Josh Swanson <joshswanson@redhat.com>