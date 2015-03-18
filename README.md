# ansible-development

My attempt to create a reproducible, isolated development environment using
Ansible.

## installation

### requirements

  * ansible 1.8.2+
  * configure your site.yml roles
  * configure your host_vars

### running

`ansible-playbook site.yml -i production`
