# ansible-git

Install git via Homebrew.

## Role Variables

User-related variables:

* `set_git_user_info`: Defaults to false.
* `git_user_name`: Will be prompted for if not set and `set_git_user_info` is true.
* `git_user_email`: Will be prompted for if not set and `set_git_user_info` is true.

Miscellaneous variables:

* `set_git_editor`: Defaults to false.
* `git_editor`: Will be prompted for if not set and `set_git_editor` is true.

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
        set_git_user_info: true
        git_user_name: xxxxx
        git_user_email: xxxxx
        set_git_editor: true
        git_editor: xxxxx
```

## License

MIT
