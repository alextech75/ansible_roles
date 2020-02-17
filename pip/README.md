# Ansible Role: Pip (for Python)

On RedHat/CentOS, you may need to have EPEL installed before running this role.

## Example Playbook
```
---
- hosts: all
    
  vars:
    pip_install_packages:
      - name: docker
  roles:
    - pip

