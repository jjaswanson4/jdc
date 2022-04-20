# Ansible Collection - network_automation.ip_address_management

A collection of automation for common CMDB related tasks. The main use case is to manage (create/update/delete) records for instances created on-premise or in a cloud provider.

# Use Cases

- Create CMDB records for instances
- Update CMDB records if instance details change
- Delete CMDB records once instances are retired

# Contents

## Roles:

- `cmdb_automation.manage_records.manage_instance_records`: Manage CMDB records, runs contextual to an instance (however the instance doesn't need to exist).

## Modules:

<none>
