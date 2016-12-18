ansible-j
=================
[![Build Status](https://travis-ci.org/dotstrap/ansible-j.svg)](https://travis-ci.org/dotstrap/ansible-j)

Configure a smarter, but not as smart as [z], [fasd], [enhancd], [j] etc., cd.

Installation
------------

```
ansible-galaxy install dotstrap.j
```

Requirements
------------

[fisherman/fzf]

Role Variables
--------------

See [default variables].

Dependencies
------------

```
- role: [ dotstrap.fzf ]
```

Example Playbook
----------------

```
- hosts: all
  roles:
    - role: dotstrap.j
```

Notes
-----

__Warning__: This role modifies your default shell configuration file, eg.
`~/.bash_profile`, `~/.zshrc` or `~/.config/fish/config.fish`.

License
-------

MIT

Author Information
------------------

[@mwilliammyers]

[@mwilliammyers]: https://github.com/mwilliammyers
[bash]: https://www.gnu.org/software/bash/manual/bashref.html
[default variables]: defaults/main.yml
[dotstrap]: https://github.com/mwilliammyers/dotstrap
[fasd]: https://github.com/clvv/fasd
[files]: files/
[fish]: http://fishshell.com/
[pure]: https://github.com/sindresorhus/pure
[variables]: vars/main.yml
[z]: https://github.com/rupa/z
[j]: https://github.com/rupa/j
[enhancd]: https://github.com/b4b4r07/enhancd
[zsh]: http://zsh.sourceforge.net
[fisherman/fzf]: https://github.com/fisherman/fzf
