Ansible NGINX Unit Role
=======================

This role installs NGINX Unit on your target host.

**Note:** This role is still in active development. There may be unidentified issues and the role variables may change as development continues.

Requirements
------------

**Ansible**

This role was developed and tested with [maintained](https://docs.ansible.com/ansible/latest/reference_appendices/release_and_maintenance.html#release-status) versions of Ansible. Backwards compatibility is not guaranteed.

Instructions on how to install Ansible can be found in the [Ansible website](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).

**Molecule**

Molecule is used to test the various functionailities of the role. Instructions on how to install Molecule can be found in the [Molecule website](https://molecule.readthedocs.io/en/latest/installation.html).

Installation
------------

**Ansible Galaxy**

Use `ansible-galaxy install nginxinc.nginx_unit` to install the latest stable release of the role on your system.

**Git**

Use `git clone https://github.com/nginxinc/ansible-role-nginx-unit.git` to pull the latest edge commit of the role from GitHub.

Platforms
---------

The NGINX Ansible role supports all platforms supported by [NGINX Unit](https://unit.nginx.org/installation/#official-packages):

```yaml
Amazon Linux:
  versions:
    - 2018.03
Amazon Linux 2:
  versions:
    - any
CentOS:
  versions:
    - 6
    - 7
    - 8
Debian:
  versions:
    - stretch
    - buster
RedHat:
  versions:
    - 6
    - 7
    - 8
Ubuntu:
  versions:
    - xenial
    - bionic
    - focal
```

Role Variables
--------------

This role has multiple variables. The descriptions and defaults for all these variables can be found in the **`defaults/main`** directory in the following files:

-   **[defaults/main/main.yml](https://github.com/nginxinc/ansible-role-nginx-unit/blob/main/defaults/main/main.yml):** NGINX Unit installation variables
-   **[defaults/main/selinux.yml](https://github.com/nginxinc/ansible-role-nginx-unit/blob/main/defaults/main/unit.yml):** NGINX Unit SELinux variables
-   **[defaults/main/bsd.yml](https://github.com/nginxinc/ansible-role-nginx-unit/blob/main/defaults/main/bsd.yml):** BSD specific installation variables

Example Playbooks
-----------------

A working functional playbook example can be found in the **`molecule/common`** directory in the following file:

**[molecule/common/playbooks/default_converge.yml](https://github.com/nginxinc/ansible-role-nginx-unit/blob/master/molecule/common/playbooks/default_converge.yml):** Install NGINX Unit

Do note that if you install this repository via Ansible Galaxy, you will have to replace the role variable in the sample playbooks from `ansible-role-nginx-unit` to `nginxinc.nginx_unit`.

Other NGINX Roles
-----------------

You can find an Ansible role to install and configure NGINX [here](https://github.com/nginxinc/ansible-role-nginx)

You can find an Ansible role to install and configure NGINX App Protect [here](https://github.com/nginxinc/ansible-role-nginx-app-protect)

You can find an Ansible collection of roles to install and configure NGINX Controller [here](https://github.com/nginxinc/ansible-collection-nginx_controller)

License
-------

[Apache License, Version 2.0](https://github.com/nginxinc/ansible-role-nginx/blob/main/LICENSE)

Author Information
------------------

[Alessandro Fael Garcia](https://github.com/alessfg)

[Tom Gamull](https://github.com/magicalyak)

&copy; [F5 Networks, Inc.](https://www.f5.com/) 2020
