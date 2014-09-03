ansible-role-ssh_config
===========================

Generate a ~/.ssh/config with your inventory (keep your old .ssh/config in backup)

Playbook example : ( file local_ssh_config.yml )
```
  ---
   - hosts: all
     sudo: no
     gather_facts: yes

   - hosts: localhost
     connection: local
     sudo: false
     roles:
      - ssh-config
```
