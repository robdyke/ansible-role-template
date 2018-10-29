# YOU.YOUR_ROLE_NAME_HERE

YOUR_ROLE_SHORT_DESCRIPTION_HERE

Requirements
------------

Python 3.5 or above (Ansible 2.5 requirement).

Role Variables
--------------

See `defaults/main.yml` and `vars/main.yml`, or the example below

Dependencies
------------

See `meta/main.yml` for other roles dependencies

Example Playbook
----------------

```yaml
---
- hosts: all
- roles:
  - role: YOU.YOUR_ROLE_NAME_HERE
    vars:
      your_role_variable_here: true
      your_role_variable_list_also_here:
        - one
        - 2
        - b'11'
```

Tests
-----

Test are made via Molecule and TestInfra. They will be automatically ran by the CI after every push. For a local run

- Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- Install [Vagrant](https://www.vagrantup.com/downloads.html)
- Open a command prompt in the repository local folder and run `vagrant up`
- Wait for it to be done starting & configuring & provionning, then `vagrant ssh`
- Once connected in the VM, testing molecule is `cd /vagrant/ansible-role-YOUR_ROLE_NAME_HERE; molecule test`

Author Information
------------------

Rémy Garrigue
