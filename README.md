# Win Auto Login
Ansible role to configure auto login on a Windows 10 machine.

## Requirements
None

## Role Variables
Available variables are listed below, along with default values `(see defaults/main.yml)`:
```yaml
auto_login_user: null
auto_login_user_password: null
```
Required variables (role will fail if the variables are not set):
```yaml
auto_login_user: "string"
auto_login_user_password: "string"
```

## Dependencies
* [check-required-variables](https://github.com/artcom/ansible-role-check-required-variables)

## Example Playbook
```yaml
- hosts: all
  tasks:
    - import_role:
        name: win-auto-login
      vars:
        auto_login_user: "{{ ansible_user }}"
        auto_login_user_password: "Sup3r5eKret"
```

## License
MIT
