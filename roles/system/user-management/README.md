system/user-management
======================

User management and privilege-escalation configuration for a Spigot game server.


Requirements
------------

This role adds a user management layer to the system configuration for a Spigot game server.
Special privileges are given to members of the `spigot-admin` group to manage and access a wider subset of the system.
In this case, the key objective is to allow the restarting of systemd services via `systemctl restart`.


Role Variables
--------------

This role uses the inherited variable `{{ admin_uids }}` to create the user accounts for the admin users, if they do not already exist.
Lists of strings are used to elevate users to use privileged commands.
`privileged.full_sudo` adds listed users to the `wheel` group, while `privileged.jr_sysadmins` adds users to the `spigot-admin` group.

```yaml
---
privileged:
  full_sudo:
	- blaster
	- jmw
	- jwf
  jr_sysadmins:
  	- dinnerbone
	- echophox
```


Dependencies
------------

Depends on the [`spigot` role](https://github.com/CrystalCraftMC/infrastructure/tree/master/roles/spigot).


License
-------

BSD-2-Clause


Author Information
------------------

This role was created in 2021 by [Justin W. Flory](https://jwf.io/).
