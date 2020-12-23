# Changelog

## 0.2.3 (Unreleased)

ENHANCEMENTS:

The GitHub actions Molecule CI/CD workflow is no longer run on a new release (this is not necessary since it already runs on every push).

## 0.2.2 (December 22, 2020)

ENHANCEMENTS:

*   Update Molecule to `3.2.1` and Docker Python SDK to `4.4.0`.
*   Remove CentOS/RHEL `6` from supported platforms due to EOL.
*   Replace TravisCI with GitHub actions.

BUG FIXES:

Fix issue whereas SELinux state would not be correctly set back to `enforcing` when `nginx_unit_selinux: true`.

## 0.2.1 (November 19, 2020)

ENHANCEMENTS:

*   Update Ansible (now Ansible base) to `2.10.3`, Ansible (now Ansible Community Distribution) to `2.10.3`, Ansible Lint to `4.3.7`, Molecule to `3.1.5`, and yamllint to `1.25.0`.
*   Moved "constant" variables to `vars/main.yml`.
*   Switch to using `ansible_facts` wherever possible.
*   Major backend refactoring to reduce the number of files and tasks.
*   Improved tasks naming conventions.
*   Add survey to README.
*   Improve README structure and use tables where relevant.

## 0.2.0 (August 27, 2020)

BREAKING CHANGES:

The repository names in Debian and RedHat based distros have slightly changed. You may run into some duplication issues when running the role on a preexisting target that already has had NGINX installed using the role. To fix this, manually remove the old repository source.

FEATURES:

TravisCI now always uses the latest version of Docker.

ENHANCEMENTS:

*   Update Ansible to `2.9.12` and Ansible Lint to `4.3.2`.
*   Explicitly define `mode` in relevant tasks.
*   Explicitly define the `nginx-unit` `apt_repository` and `yum_repository` filename in Debian and RedHat based distros.

## 0.1.0 (August 19, 2020)

Initial release of the NGINX Unit role. Contains all NGINX Unit related features previously available on the [NGINX Ansible role](https://github.com/nginxinc/ansible-role-nginx).
