# NGINX automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-nginx
  name: ansible-role-nginx
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-nginx

- Import role and override role variables, e.g.
```
- name: Setup nginx
  roles:
    - role: ansible-role-nginx
```

- All available role vars can be found in `defaults`
