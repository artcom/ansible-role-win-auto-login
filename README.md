# Win Auto Login
Ansible role to configure auto login on a Windows 10 machine.

## Role Variables
Available variables are listed below, along with default values `(see defaults/main.yml)`:
```yaml
auto_login_user: null
auto_login_user_password: null
```

Mandatory variables (role will fail if the variables are not set):
```yaml
auto_login_user: "string"
auto_login_user_password: "string"
```
