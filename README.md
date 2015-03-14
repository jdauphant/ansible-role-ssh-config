ansible-role-ssh_config
===========================

Generate a ~/.ssh/config with your inventory (keep your old .ssh/config in backup)

Available on Ansible Galaxy : https://galaxy.ansible.com/list#/roles/3116

# Playbook example :
```
  ---
   - hosts: all
     sudo: no
     gather_facts: yes

   - hosts: localhost
     connection: local
     sudo: false
     roles:
      - jdauphant.ssh-config
```
# Notes
- You need to gather_facts of your hosts before the run the role in local
- You old .ssh/config is keep in backup and integrated to the new .ssh/config
