ansible-role-foreman
=========

# Description
Ansible role to manage Foreman resources. This role does not install Foreman!

The following resources can be managed (currently only created or deleted).
- Architectures
- Compute Attributes
- Compute Profiles
- Compute Resources
- Config Templates
- Domains
- Environments
- Hostgroups
- Hosts
- Locations
- Media
- Operatingsystems
- Organizations (requires Katello)
- Roles
- Smart Proxies
- Subnets
- Users

# Requirements
Ansible is required as well as the [Ansible library] to manage Foreman resources.

# Role Variables

| Name | Description | Default value |
| :------ | :------ | :----- |
| foreman_debug | Boolean to define if results of each task should be printed | False |
| foreman_default_domain | Default Domain of a host if not specified | None |
| foreman_default_environment | Default Environment of a host if not specified | None |
| foreman_default_location | Default Location of a host if not specified | None |
| foreman_default_hostgroup | Default Hostgroup of a host if not specified | None |
| foreman_default_operatingsystem | Default Operatingsystem of a host if not specified | None |
| foreman_default_organization | Default Organization of a host if not specified | None |
| foreman_default_compute_profile | Default Compute Profile of a host if not specified | None |
| foreman_default_compute_resource | Default Compute Resource of a host if not specified | None |

# Dependencies

No other roles needed

# Example Playbooks
```yaml
- hosts: foreman
  roles:
   - role: foreman
```
# License

BSD

Author Information
------------------
[Thomas Krahn]: mailto:ntbc@gmx.net

[Ansible library]: https://github.com/Nosmoht/ansible-library-foreman
