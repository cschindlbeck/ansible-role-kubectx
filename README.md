# ansible-role-kubectx

![Ansible](https://github.com/avnes/ansible-role-kubectx/actions/workflows/ansible.yaml/badge.svg)

Ansible role for installing kubectx.

## Requirements

Poetry. Install it from <https://python-poetry.org/docs/>

## Role Variables

```yaml
kubectx_version: 3.7.2
kubectx_for_all_users: true # If false it will install in in the users ~/bin directory
command_shell: bash         # Must be bash or zsh
```

## Dependencies

None

## Example Playbook

```yaml
- hosts: all
  roles:
     - { role: avnes.kubectx }
```

## For pip compability

```bash
poetry export --dev --output requirements.txt
```

## Test

```bash
poetry install
poetry shell
molecule test
```

## License

MIT

## Author Information

<https://github.com/avnes>
