# Ansible Role: ansible-apps_flexera

## Description

[![Build Status](https://travis-ci.com/lotusnoir/ansible-apps_flexera.svg?branch=master?style=flat)](https://travis-ci.com/lotusnoir/ansible-apps_flexera)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)
[![Ansible Role](https://img.shields.io/badge/galaxy-apps_flexera-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_flexera)
![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_flexera?color=orange&style=flat)
![Ansible Quality Score](https://img.shields.io/ansible/quality/52300)
[![downloads](https://img.shields.io/ansible/role/d/52300)](https://galaxy.ansible.com/lotusnoir/apps_flexera)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_flexera.svg)](https://github.com/lotusnoir/ansible-apps_flexera/releases/)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_flexera&metric=alert_status)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_flexera)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_flexera&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_flexera)
[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_flexera&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_flexera)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_flexera&metric=security_rating)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_flexera)

Deploy [flexera](https://adva.com/) the ADVA license server.

## Role variables

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `flexera_version` | 0.3.2 | flexera version |
| `flexera_install_dir` | /usr/local/bin | directory to install binary |
| `flexera_force_install` | false | force install variable |
| `flexera_user` | admin | prism user |
| `flexera_group` | admin | prism user |

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
