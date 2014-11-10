# Ansible Role: MySQL

[![Build Status](https://travis-ci.org/Aplyca/ansible-role-mysql.svg?branch=master)](https://travis-ci.org/Aplyca/ansible-role-mysql)
[![Circle CI](https://circleci.com/gh/Aplyca/ansible-role-mysql.png?style=badge)](https://circleci.com/gh/Aplyca/ansible-role-mysql)

Ansible Role that installs an configure MySQL on Debian/Ubuntu.

## Requirements

Use hash behavior for variables in ansible.cfg
See example: https://github.com/Aplyca/ansible-role-mysql/blob/master/tests/ansible.cfg
See official docs: http://docs.ansible.com/intro_configuration.html#hash-behaviour

## Installation

Using ansible galaxy:
```bash
ansible-galaxy install mauricios.MySQL
```
You can add this role as a dependency for other roles, add the role to the meta/main.yml file of your own role:
```yaml
dependencies:
  - { role: mauricios.MySQL }
```

## Role Variables

See default variables: https://github.com/Aplyca/ansible-role-mysql/blob/master/defaults/main.yml

## Dependencies

None.

## Testing

Use Vagrant to test the role:

```bash
cd tests;
vagrant box add ubuntu/trusty64;
vagrant up;
```
You should see a MySQL server on localhost:3306

## License

MIT / BSD

## Author Information

Mauricio Sánchez from Aplyca SAS (http://www.aplyca.com)