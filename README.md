# Ansible script to configurate your personal pc 

## Prerequisite

You need install ansible. **Recommended** you should use provide Pipenv.

## How run

If you want run this ansible locally you can use default playbook, if you want it on remote machine see ansible documentation how you can set up your playbook (hosts).
```
pipenv run ansible-playbook <clear-linux/ubuntu>/playbook.yml -K -u $USER
```
