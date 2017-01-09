# Ansible role for `anyenv` of user

- Setup [anyenv](https://github.com/riywo/anyenv)
- Setup [rbenv](https://github.com/rbenv/rbenv)
- And some plugins

## Requirements

- Debian
- Ubuntu

## Role Variables

- `anyenv_home_dir`: path to user's home directory
- `git_update`: `update` option of [git module](http://docs.ansible.com/git_module.html)
- `git_depth`: `depth` option of [git module](http://docs.ansible.com/git_module.html)

## Dependencies

None.

## Example Playbook

Normal usage:

    ---
    - hosts: all
      become: no
      roles:
      - znz.user-dot-shell

## Example requirements.yml

    - src: https://github.com/znz/ansible-role-user-dot-shell
      version: master
      name: znz.user-dot-shell

## License

MIT License
