
# Home Lab Ansible

This is a repo for my local home lab, to limit the amount of changes I have to apply after I properly bork my local instances.


# Order of Ops
1. run localhost_ssh.yml to generate local ssh keys
2. run distribute_ssh.yml to distribute those keys to the various servers


# Example Run 
```bash
  ansible-playbook playbooks/mount.yml --ask-become-pass --ask-vault-pass -i ./inventory/hosts 
```
