# K8_CLUSTER_ANSIBLE

  # INTEGRATING AMAZON-WEB-SERVICES, KUBERNETES and ANSIBLE.

## This repo contains three ansile roles
### 1. ec2_instance.
### 2. master_node.
### 3. worker_node.

## PRE-REQUISITES 
    language: python
    python: "2.7"

### Use the new container infrastructure
      sudo: false

### Install ansible
    addons:
      apt:
        packages:
        - python-pip

install:
  ### Install ansible
      - pip install ansible

  ### Check ansible version
      - ansible --version

  ### Create ansible.cfg with correct roles_path
      - printf '[defaults]\nroles_path=../' >ansible.cfg

script:
  ### Basic role syntax check
      - ansible-playbook tests/test.yml -i tests/inventory --syntax-check
