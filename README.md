# Ansible script to configurate your personal pc 

## Prerequisite

You need install ansible. **Recommended** you should use provide Pipenv.

## How run

If you want run this ansible locally you can use default playbook, if you want it on remote machine see ansible documentation how you can set up your playbook (hosts).

**ClearLinux**
```bash
pipenv run ansible-playbook clear_linux/playbook.yml -K -u $USER
```

**Ubuntu**
```bash
pipenv run ansible-playbook ubuntu/playbook.yml -i ubuntu/inventory.yml -K -u $USER
```
