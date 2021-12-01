# ansible-apps_flexera

## Description

[![Galaxy Role](https://img.shields.io/badge/galaxy-apps_flexera-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_flexera)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_flexera.svg)](https://github.com/lotusnoir/ansible-apps_flexera/releases/latest)
![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_flexera?color=orange&style=flat)
[![downloads](https://img.shields.io/ansible/role/d/56092)](https://galaxy.ansible.com/lotusnoir/apps_flexera)
![Ansible Quality Score](https://img.shields.io/ansible/quality/56092)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)

Deploy [flexera](https://adva.com/) the ADVA license server.

## Requirements

none

## Role variables

See [variables](/defaults/main.yml) for more details.

## Examples

        ---
        - hosts: apps_flexera
          become: true
          become_method: sudo
          gather_facts: true
          roles:
            - role: ansible-apps_flexera


## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.

