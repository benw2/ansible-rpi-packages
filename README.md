# Ansible Role: Raspberry Pi Packages

Quick ansible role to install common RPI packages, and setup unattended upgrades

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
rpi_packages:
  # To allow for unattended upgrades, set this to true
  unattended_upgrades: false
  # List of common packages to install
  common_packages:
  - ca-certificates
  - curl
  - dnsutils
  - git
  - htop
  - python3
  - python3-pip
  - rsync
  - traceroute
  - unattended-upgrades
  - wget
```

To override :

```yaml
rpi_packages.unattended_upgrades: true
rpi_packages.common_packages:
- ansible
```

## Dependencies

None

