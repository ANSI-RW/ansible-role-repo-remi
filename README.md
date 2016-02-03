# Ansible Role: Remi Repository

[![Build Status](https://img.shields.io/travis/thestarkenya/ansible-role-repo-remi.svg)](https://travis-ci.org/thestarkenya/ansible-role-repo-remi) [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/thestarkenya/ansible-role-repo-remi/master/LICENSE)

Installs the Remi repository (Les RPM de Remi) on RHEL/CentOS.

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
# Remi repo GPG key
remi_repo_gpg_key_url: http://rpms.remirepo.net/RPM-GPG-KEY-remi
# Remi repo package
remi_repo_url: http://rpms.famillecollet.com/enterprise/remi-release-{{ ansible_distribution_major_version }}.rpm
```

## Dependencies

None

## Example Playbook

```yaml
- hosts: servers

  roles:
    - role: ansible-role-repo-remi
```

## License

MIT
