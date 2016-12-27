# Ansible for the RTB Project

[Ansible Documentation](http://docs.ansible.com/ansible/index.html)

We use [Vault](http://docs.ansible.com/ansible/playbooks_vault.html) to store passwords and secrets. 

Hosts and their roles are defined in the [inventory](http://docs.ansible.com/ansible/intro_inventory.html)


## Getting Started

You need a hosts with python, and ansible 2.2 or higher installed.

You need to [configure](http://docs.ansible.com/ansible/intro_configuration.html) ansible to fit your system. The included `ansible.cfg` might or might not work for yours.

### Installing all required roles
```
ansible-galaxy install -r requirements.yml
```

## Running Ansible

  * ```ansible-playbook site.yml``` will apply all settings to all hosts
  * ```ansible-playbook site.yml -l stats``` will apply all settings, but only to the stats hosts