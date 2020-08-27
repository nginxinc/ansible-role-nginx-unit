# Changelog

## 0.2.0 (August 27, 2020)

BREAKING CHANGES:

*   The repository names in Debian and RedHat based distros have slightly changed. You may run into some duplication issues when running the role on a preexisting target that already has had NGINX installed using the role. To fix this, manually remove the old repository source.

ENHANCEMENTS:

*   Update Ansible to `2.9.12` and Ansible Lint to `4.3.2`.
*   Explicitly define `mode` in relevant tasks.
*   Explictly define the `nginx-unit` `apt_repository` and `yum_repository` filename in Debian and RedHat based distros.

## 0.1.0 (August 19, 2020)

Initial release of the NGINX Unit role. Contains all NGINX Unit related features previously available on the [NGINX Ansible role](https://github.com/nginxinc/ansible-role-nginx).
