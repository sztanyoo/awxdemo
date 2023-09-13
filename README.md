# awxdemo
A repository to store example playbooks for an AWX demo


## Custom secret

**Input configuration**
```
fields:
  - id: username
    type: string
    label: Username
  - id: password
    type: string
    label: Password
    secret: true
```

**Injector configuration**
```
extra_vars:
  service_username: '{{ username }}'
  service_password: '{{ password }}'
```
