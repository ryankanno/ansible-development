[![Build Status](https://travis-ci.org/ryankanno/ansible-development.svg?branch=master)](https://travis-ci.org/ryankanno/ansible-development)

# ansible-development

A reproducible, isolated development environment using Ansible.

## installation

### requirements

  - install [ansible 1.8.2+](http://docs.ansible.com/intro_installation.html#installation)
  - configure your site.yml roles ([site.yml](https://github.com/ryankanno/ansible-development/blob/master/site.yml))
  - configure your inventory file ([production.example](https://github.com/ryankanno/ansible-development/blob/master/production.example))
  - configure your host_vars file ([localhost.example](https://github.com/ryankanno/ansible-development/blob/master/host_vars/localhost.example))

#### installing ansible
#### configure your site.yml
#### configure your inventory file
#### configure your host_vars file

### running

#### displaying ansible variables about your machine

`ansible devmachine -i production -m setup --connection=local`

#### running the playbook

`ansible-playbook site.yml -i production --connection=local --ask-sudo-pass`

# todo

  - add in homebrew role
      - add https://github.com/zmap/zmap
      - add https://github.com/keycastr/keycastr
