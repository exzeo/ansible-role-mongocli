Ansible Role Mongo
=========

Installs Mongo/Mongo-cli on Debian/Ubuntu servers. 

Role Variables
--------------

```
# Mongo Version to install
mongo_version: ""

# Toggling this will uninstall from the server
uninstall: false
```

Example Playbooks
----------------

Minimal:
```
- name: Install Docker
  hosts: all
  roles:
    - role: exzeo.mongocli
```

Specific Version:
```
- name: Install Docker
  hosts: all
  roles:
    - role: exzeo.mongocli
      vars:
        mongo_version: "5.0.5"
```

Uninstall:
```
- name: Install Docker
  hosts: all
  roles:
    - role: exzeo.mongocli
      vars:
        uninstall: true
```