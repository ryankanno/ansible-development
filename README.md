# ansible-development

My attempt to create a reproducible, isolated development environment using
Ansible.

## installation

### requirements

  * ansible 1.8.2+
  * configure your site.yml roles ([site.yml](https://github.com/ryankanno/ansible-development/blob/master/site.yml))
  * configure your inventory file ([production.example](https://github.com/ryankanno/ansible-development/blob/master/production.example))
  * configure your host_vars file ([localhost.example](https://github.com/ryankanno/ansible-development/blob/master/host_vars/localhost.example))

### running

`ansible-playbook site.yml -i production --connection=local`
