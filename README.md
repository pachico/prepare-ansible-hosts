# Prepare ansible hosts

Provision Debian based machines to be Ansible targets.
It installs Python 2, copies ssh keys and locales.

## Requirements

* Ansible (tested in version 2.7.7)
* Debian based machines to provision

## How to run it

1. Clone or download this repo
2. Rename `inventory.dist` to `inventory`
3. Edit `inventory` setting the IPs of the machines you want to provision
4. Run playbook:

```bash
ansible-playbook ./playbook.yml -i inventory --ask-pass -u ubuntu --ask-become-pass
```

## Credits

Thanks to [Dave Cohen](https://github.com/groovemonkey) for his course and ideas!
