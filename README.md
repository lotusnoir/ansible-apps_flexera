# ansible-apps_flexera

## Description

[![Galaxy Role](https://img.shields.io/badge/galaxy-apps_flexera-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_flexera)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_flexera.svg)](https://github.com/lotusnoir/ansible-apps_flexera/releases/latest)
![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_flexera?color=orange&style=flat)
[![downloads](https://img.shields.io/ansible/role/d/56092)](https://galaxy.ansible.com/lotusnoir/apps_flexera)
![Ansible Quality Score](https://img.shields.io/ansible/quality/56092)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)

Deploy [flexera](https://adva.com/) the ADVA license server.

## Role variables

| Name                    | Default Value | Description                        |
| ----------------------- | ------------- | -----------------------------------|
| `flexera_version`       | 2.3.1         | flexera version |
| `flexera_source_file`   | ""            | application package |
| `flexera_install_dir`   | /opt          | installation directory |
| `flexera_force_install` | false         | force install variable |
| `flexera_user`          | flexnetls     | prism user |
| `flexera_group`         | flexnetls     | prism user |
| `flexera_config_firewalld` | true    | Open port on firewalld |

## Examples

	---
	- hosts: apps_flexera
	  become: yes
	  become_method: sudo
	  gather_facts: yes
	  roles:
	    - role: ansible-apps_flexera
	  environment: 
	    http_proxy: "{{ http_proxy }}"
	    https_proxy: "{{ https_proxy }}"
	    no_proxy: "{{ no_proxy }}

## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.
