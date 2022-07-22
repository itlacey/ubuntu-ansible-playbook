
# Home Lab Ansible

This is a repo for my local home lab, to limit the amount of changes I have to apply after I properly bork my local instances.
This setups up various docker images that I use and run in my home lab, as well as mounts persistent files to the servers via s3fs (storing the files in s3)

# Order of Ops
1. run localhost_ssh.yml to generate local ssh keys
2. run distribute_ssh.yml to distribute those keys to the various servers


# Example Run 
```bash
  ansible-playbook playbooks/mount.yml --ask-become-pass --ask-vault-pass -i ./inventory/hosts 
```
