# Ansible Role: Plantd Configure

<!--[![Build Status](https://img.shields.io/travis/geoffjay/ansible-plantd-configure/master.svg?style=flat)](https://travis-ci.org/geoffjay/ansible-plantd-configure-->
<!--[![stability-stable](https://img.shields.io/badge/stability-stable-green.svg?style=flat)](https://github.com/orangemug/stability-badges)-->
[![Ansible Galaxy](https://img.shields.io/ansible/role/36021.svg?style=flat)](https://galaxy.ansible.com/geoffjay/plantdconfigure)
[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://raw.githubusercontent.com/geoffjay/ansible-plantd-configure/master/LICENSE)

[WIP] Pre-alpha, doesn't work.

Installs and configures a Plantd configure server on a Debian host.

## Requirements

A working installation of `go`.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yml
plantd_configure_version: "0.1.0"
```

## Dependencies

None

## Example Playbook

```yml
- hosts: master
  become: yes
  vars_files:
    - vars/main.yml
  roles:
    - geoffjay.plantdconfigure
```

Inside `vars/main.yml`:

```yml
plantd_configure_version: "0.1.0"
```

## License

MIT/BSD

## Author Information

This role was created in 2019 by Geoff Johnson.
