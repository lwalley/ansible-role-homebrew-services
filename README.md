# Ansible Role: Homebrew Services

Ensures services managed by [Homebrew][brew] start at login on Mac OS X.

Temporary role until homebrew services is included in geerlinguy.homebrew, see
# https://github.com/geerlingguy/ansible-role-homebrew/issues/65.

## Requirements

[Homebrew][brew] and its services  must be installed on the system prior to
running this role (suggested role: `geerlingguy.homebrew`).

## Role Variables

Available variables with example values are listed below, for default values see
[`defaults/main.yml`](defaults/main.yml)):

    homebrew_services:
      - dnsmasq

## Dependencies

None.

## Example Playbook

    - hosts: localhost
      roles:
         - { role: lwalley.homebrew-services }

## License

MIT

[Hombrew]: https://brew.sh
