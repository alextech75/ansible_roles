# Ansible Postgres Docker

Run Postgres inside a Docker container

## Dependencies

- pip
- Docker

## Example Playbook

```yaml
- hosts: servers
  become: true
  roles:
    - pip
    - docker
    - postgres_docker
```
