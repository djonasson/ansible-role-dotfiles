# Ansible Role: Dotfiles

[![CI](https://github.com/djonasson/ansible-role-dotfiles/workflows/CI/badge.svg?event=push)](https://github.com/djonasson/ansible-role-dotfiles/actions?query=workflow%3ACI)

Ansible role for installing dotfiles from a git repository.

## Requirements

Requires `git` on the managed machine.

## Role Variables

The role variables are defined in `defaults/main.yml` with these defaults:

    repo: "https://github.com/djonasson/dotfiles.git"
    dest: "~/.dotfiles"
    version: master
    accept_hostkey: false
    installation_dir: "~"

## Dependencies

None

## Example Playbook

    - hosts: localhost
      roles:
        - role: djonasson.dotfiles

## License

MIT

## Author

This ansible role was created by [Daniel Jonasson](https://github.com/djonasson/).
