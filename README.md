# Ansible_roles
test with molecule

https://molecule.readthedocs.io/en/latest/installation.html

To test a role, change directory into the role to test, and execute Molecule as follows.

```
docker run --rm -it \
    -v "$(pwd)":/tmp/$(basename "${PWD}"):ro \
    -v /var/run/docker.sock:/var/run/docker.sock \
    -w /tmp/$(basename "${PWD}") \
    quay.io/ansible/molecule:2.22 \
    molecule test

