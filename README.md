# Local computer

Setup local computer configuration

1. Various command line

It supports the following OS

1. OSX (ARM)

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
