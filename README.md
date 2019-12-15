# Ansible Role: docker

[![Build Status](https://img.shields.io/travis/arillso/ansible.docker.svg?branch=master&style=popout-square)](https://travis-ci.org/arillso/ansible.docker) [![license](https://img.shields.io/github/license/mashape/apistatus.svg?style=popout-square)](licence) [![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-docker-blue.svg?style=popout-square)](https://galaxy.ansible.com/arillso/docker) [![Ansible Role](https://img.shields.io/ansible/role/d/30744.svg?style=popout-square)](https://galaxy.ansible.com/arillso/docker)

## Description

Installed and Configuriet then docker deamon on different Linux systems.

## Installation

```bash
ansible-galaxy install arillso.docker
```

## Requirements

None

## Role Variables

| Variable           | Default | Comments (type)                                             |
| :----------------- | :------ | :---------------------------------------------------------- |
| docker_daemon      | []      | Configure the daemon.json file from docker.                 |
| docker_cron_enable | true    | Creates a cronjob that deletes the old image and container. |

## Dependencies

None

## Example Playbook

```yml
- hosts: all
  roles:
    - arillso.docker
```

## Author

- [Simon Bärlocher](https://sbaerlocher.ch)
- [mleutenegger](https://github.com/mleutenegger)

## License

This project is under the MIT License. See the [LICENSE](https://sbaerlo.ch/licence) file for the full license text.

## Copyright

(c) 2020, Arillso
