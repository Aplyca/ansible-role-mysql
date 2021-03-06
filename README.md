# Ansible Role: MySQL

[![Build Status](https://travis-ci.org/Aplyca/ansible-role-mysql.svg?branch=master)](https://travis-ci.org/Aplyca/ansible-role-mysql)
[![Circle CI](https://circleci.com/gh/Aplyca/ansible-role-mysql.svg?style=svg)](https://circleci.com/gh/Aplyca/ansible-role-mysql)

Ansible Role that installs an configure MySQL on Debian/Ubuntu.

## Requirements

Use hash behavior for variables in ansible.cfg
See example: https://github.com/Aplyca/ansible-role-mysql/blob/master/tests/ansible.cfg
See official docs: http://docs.ansible.com/intro_configuration.html#hash-behaviour

## Installation

Using ansible galaxy:
```bash
ansible-galaxy install aplyca.MySQL
```
You can add this role as a dependency for other roles, add the role to the meta/main.yml file of your own role:
```yaml
dependencies:
  - { role: aplyca.MySQL }
```

Use `merge` hash behaviour for variables like dictionaries in Python. You can set this configuration by adding the setting `hash_behaviour=merge` to the `ansible.cfg` file which should be placed in the same directory where you are executing ansible-playbook command. See the docs for more info: http://docs.ansible.com/ansible/intro_configuration.html#hash-behaviour or see the example here: https://github.com/Aplyca/ansible-role-mysql/blob/master/ansible.cfg

## Role Variables

See default variables: https://github.com/Aplyca/ansible-role-mysql/blob/master/defaults/main.yml

## Dependencies

None.

## Testing

### Vagrant
* You can use Vagrant to set up and provision a VM in order to run tests.
* To know more about Vagrant: http://www.vagrantup.com
  And Vagrant with Ansible: http://docs.vagrantup.com/v2/provisioning/ansible.html

```bash
tests/vagrant.sh
```
### Docker

```bash
tests/docker.sh
```
