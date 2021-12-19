[![Build Status](https://travis-ci.org/ryankanno/ansible-development.svg?branch=master)](https://travis-ci.org/ryankanno/ansible-development)

# ansible-development

A reproducible, isolated development environment using Ansible.

## installation

### requirements

  - install [ansible 5.x+](http://docs.ansible.com/intro_installation.html#installation)
  - configure your site.yml roles ([site.yml](https://github.com/ryankanno/ansible-development/blob/master/site.yml))
  - configure your inventory file ([production.example](https://github.com/ryankanno/ansible-development/blob/master/production.example))
  - configure your host_vars file ([localhost.example](https://github.com/ryankanno/ansible-development/blob/master/host_vars/localhost.example))
  - ansible-galaxy install -r requirements.yml

### running

#### displaying ansible variables about your machine

`ansible devmachine -i production -m setup

#### running the playbook

`ansible-playbook site.yml -i production -K`

`arch -arm64e ansible-playbook site.yml -i production -K`

`arch -arm64e ansible-playbook site.yml -i production -K --tags macports`
