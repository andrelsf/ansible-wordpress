# Vagrant and Ansible

### TODO
- [x] HTTD
- [x] PHP-FPM
- [x] MySQLServer

## Atividade MIT DevOps e Cloud SENAI FATESG

* Requirimentos
    - Virtualbox 6.x

Provisionamento de uma instancia AlmaLinux8 usando Ansible playbook para configurar e implementar ambiente com WordPress.

### Renomei o arquivo ou copie
 - [mysql-vars.yml.example](files/ansible/vars/mysql-vars.yml.example) => [mysql-vars.yml](files/ansible/vars/mysql-vars.yml)

### Atualize o arquivo para suas credenciais customizadas.
 - [mysql-vars.yml](files/ansible/vars/mysql-vars.yml)
```
DB_HOST: 192.168.56.201
MYSQL_ROOT_PASSWORD: YOUR_ROOT_SECRET
WORDPRESS_DATABASE: YOUR_DATABASE
WORDPRESS_USER: YOUR_USER_DB
WORDPRESS_USER_PASSWORD: YOUR_USER_DB_PASSWD
```

### Execute:
```shell
vagrant up --provider virtualbox
vagrant status
```

### Acessando:

* [Worpress Local](http://192.168.56.200/wordpress)


