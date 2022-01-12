# manage_firewall_state
Role to set the firewall (typically firewalld) to the desired state.

# Inputs
This role has secure default values, however the desired state can be input like so:
```yaml
firewall:
  name: firewalld
  state: stopped
  enabled: no
```