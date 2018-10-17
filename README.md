# ansible provisioning examples for bIT ET 2018/04

Some basic examples to show how to work with ansible roles.
Based on [the vagrant virtual machine setup](https://github.com/maschmann/bit-et1804-vagrant-example).

## prerequisites

install:

- ```ansible-galaxy install tecris.maven``` for webservers
- ```ansible-galaxy install geerlingguy.mysql``` for database servers 

## commands

- ```ansible-playbook -i inventory provision.yml```
- ```ansible-playbook -i inventory provision.yml --limit webservers```
- ```ansible-playbook -i inventory provision.yml --limit webservers --tags=java```

## sources

- [Maven](https://github.com/tecris/ansible-maven)