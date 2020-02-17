# Ansible Role: Nginx

Installs Nginx on RedHat/CentOS, Debian/Ubuntu servers.

The user under which Nginx will run. Defaults to `nginx` for RedHat, `www-data` for Debian.


## Overriding configuration templates

You can override the template used to generate the virtualhost configuration files or the `nginx.conf` file.

```yaml
nginx_conf_template: "nginx.conf.j2"
nginx_vhost_template: "vhost.j2"
```

## Example Playbook

```yaml

- hosts: server
  roles:
    - nginx

