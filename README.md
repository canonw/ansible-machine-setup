# Local computer

Setup local computer configuration

1. Bash configuration
2. ZSH configuration
3. Various command line

It supports the following OS

1. OSX (ARM)

TODO: Add Ubuntu
https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html#installing-ansible-on-ubuntu


To confirm ansible setup correctly, execute

``` sh
ansible localhost -i inventory.ini -m ping
```

To dump enviornment variables, run

``` sh
ansible-playbook -i inventory.ini playbook.yml --tags "debug_info"
```

To execute computer setup, run

``` sh
ansible-playbook --ask-become-pass -i inventory.ini playbook.yml
```
