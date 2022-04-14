# Role README

This role grabs an available IP address from IPAM (Netbox), automatically allocating it to a device in the IPAM's DB.

# Inputs

The role expects the following inputs:

- `network_prefix`: What network to assign an address from, such as `10.15.120.0/22`
- `tenant`: What tenant will own this IP address, such as `RHEL Servers`

Run this role in the context of your end device, as the role will automatically delegate to localhost (or another specified host) and use `inventory_hostname`.

# Outputs
The role registers the variable `allocated_ip_address`, which contains the returned information from IPAM.

# Credentials

Assign the `Netbox Credentials` to your job template in Automation Controller to authenticate to IPAM.
