[![Build Status](https://travis-ci.com/calvinbui/ansible-nextcloud-docker.svg?branch=master)](https://travis-ci.com/calvinbui/ansible-nextcloud-docker)
![GitHub release](https://img.shields.io/github/release/calvinbui/ansible-nextcloud-docker.svg)
![Ansible Quality Score](https://img.shields.io/ansible/quality/42341.svg)
![Ansible Role](https://img.shields.io/ansible/role/d/42341.svg)

# Ansible NextCloud Docker

NextCloud in Docker. Option to also build NextCloud Docker Image based on the official [NextCloud Docker examples](https://github.com/nextcloud/docker#adding-features).

##  Requirements

N/A

## Role Variables

`nextcloud_name`: Name of container

`nextcloud_image`: Docker image to  use

`nextcloud_ports`: List of ports to expose

`nextcloud_volumes`: Volumes to mount

`nextcloud_environment_variables`: Docker environmental variables

`nextcloud_docker_additional_options`: [Additional parameters](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html) to add to docker container

## Dependencies

N/A

## Example Playbook

```yaml
- hosts: servers
  become: true
  roles:
   - role: calvinbui.ansible_nextcloud_docker
```

## License

GPLv3

## Author Information

http://calvin.me
