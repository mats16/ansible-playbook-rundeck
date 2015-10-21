# ansible-playbook-rundeck
Nginx &amp; JAVA7 on Ubuntu 14.04 LTS

## Install Ansible Roles

```shell
$ ansible-galaxy install -r requirements.yml -p roles -f
```

### Role List

- [Nginx](https://github.com/mats116/ansible-role-nginx)
- [Rudeck](https://github.com/mats116/ansible-role-rundeck)
- [MariaDB](https://github.com/mats116/ansible-role-mariadb-server) # when "mysql.host == 'localhost'"

## Launch WordPress Server on VirtualBox

### 1. Launch Server

```shell
$ vagrant up
```

### 2. Access to Rundeck

- http://127.0.0.1:10080/
