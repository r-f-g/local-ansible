# Ansible script to configurate your personal pc 

## Prerequisite

You need install all requirements. The **recommended** way is to install it in
a virtualenv.

```bash
virtualenv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## How run

If you want to run this ansible locally you can use default playbook, if you want it on remote machine see ansible documentation how you can set up your playbook (hosts).

**ClearLinux**
```bash
ansible-playbook clear_linux/playbook.yml -K -u $USER
```

**Ubuntu**
```bash
ansible-playbook ubuntu/playbook.yml -i ubuntu/inventory.yml -K -u $USER
```

Run only user settings.

```bash
ansible-playbook ubuntu/playbook.yml -i ubuntu/inventory.yml -K -u $USER --tags user-settings
```
