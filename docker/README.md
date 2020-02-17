# Ansible Role: Docker

## Use with Ansible (and `docker` Python library)

If use Ansible to then _build_ Docker images and manage Docker containers on the server where Docker is installed. In this case, you can add in the `docker` Python library using the `pip` role:

```yaml
- hosts: all

  vars:
    pip_install_packages:
      - name: docker

  roles:
    - pip
    - docker
```

## Example Playbook

```yaml
- hosts: all
  roles:
    - docker
```
