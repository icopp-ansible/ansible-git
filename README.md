# ansible-git

Install git via Homebrew.

## Role Variables

* `git_user_name`: If supplied, will be used to set a global `user.name` value for git.
* `git_user_email`: If supplied, will be used to set a global `user.email` value for git.
* `git_editor`: If supplied, will be used to set a global `core.editor` value for git.

## Dependencies

* [icopp.homebrew](https://github.com/icopp/ansible-homebrew)

## Example Playbook

```
  - hosts: all
    roles:
      - role: icopp.git
```

```
  - hosts: all
    roles:
      - role: icopp.git
        git_user_name: xxxxx
        git_user_email: xxxxx
        git_editor: xxxxx
```

## License

MIT
