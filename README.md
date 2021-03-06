# Ansible Role: Tor

[![Build Status][travis-build-status]][travis-tests] [![Ansible Role][ansible-role-shield]][ansible-role]

This role installs [Tor] on a RedHat or Debian-based linux system.

## Requirements

None.

## Dependencies

None.

## Role Variables

See [`defaults/main.yml`][defaults] for all available variables.

## Example Playbook

    - hosts: servers
      vars_files:
        - vars/main.yml
      roles:
        - noplanman.tor

*Inside `vars/main.yml`*:

    tor_http_port: "8080"

## Tests

Docker is used to test the role with different operating systems.

Check the [`tests`] folder.

## License

MIT   
Forked from https://git.feneas.org/noplanman/ansible-role-tor

[travis-build-status]: https://api.travis-ci.org/haghighi-ahmad/ansible-role-tor.svg?branch=master&style=flat-square "Travis-CI Build Status"
[travis-tests]: https://travis-ci.org/haghighi-ahmad/ansible-role-tor "Travis-CI Tests"
[ansible-role-shield]: https://img.shields.io/ansible/role/42361.svg?style=flat-square "Tor on Ansible Galaxy"
[ansible-role]: https://galaxy.ansible.com/haghighi_ahmad/tor "Tor on Ansible Galaxy"
[Tor]: https://www.torproject.org/ "Tor Project"
[defaults]: https://github.com/haghighi-ahmad/ansible-role-tor/blob/master/defaults/main.yml "Default variables"
[`tests`]: https://github.com/haghighi-ahmad/ansible-role-tor/tree/master/tests "Tests"
