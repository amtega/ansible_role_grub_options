# role_name

This is an [Ansible](http://www.ansible.com) role to setup GRUB bootloader.

## Requirements

- Ansible >= 2.4

## Role Variables

A list of all the default variables for this role is available in `defaults/main.yml`.

## Dependencies

None.

Playbook uses grubby program. Checks if it is installed, otherwise playbook install it.

## Example Playbook

```yaml
---

  - hosts: servers
    become: true
    roles:
    - role: amtega.grub
```


## Testing

Test are based on docker containers. You can run the tests with the following commands:

```shell
$ cd amtega.grub/tests
$ ansible-playbook main.yml -K

## License

Copyright (C) <YEAR> AMTEGA - Xunta de Galicia

This role is free software: you can redistribute it and/or modify
it under the terms of:
GNU General Public License version 3, or (at your option) any later version;
or the European Union Public License, either Version 1.2 or – as soon
they will be approved by the European Commission ­subsequent versions of
the EUPL;

This role is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details or European Union Public License for more details.

## Author Information

- Carlos Chedas Fernandez.
