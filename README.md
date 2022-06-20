Git Commands to become a pro
============
_Great git commands for improve your skills ...and that sometimes I forget_

## Daily commands
| Command | Description |
| ------- | ----------- |
|`git add . -p`| allows to stage piece of code |
|`git stash show -p` | show diff in last stash|
|`git stash show -p stash@{1}` | show diff in stash@{1}|
|`git checkout -- <file>`| WARNING revert the `<file>` in working directory. It is distructive command |

## Basic Configuration

### Init config

| Command | Description |
| ------- | ----------- |
| `git config --local credential.helper store` | Store password forever |
| `git config --system core.editor vim` | Set vim editor for system |

### Custom config
| Task | Command | Description |
| ---- | ------- | ----------- |
| Create alias |`git config --global alias.s 'status'`|Add alias `s` for call `git status` with `git s` (also with autocomplete)|

### System level

Stored in `/etc/gitconfig` (if present). Need sudo permissions.

| Command | Description |
| ------- | ----------- |
| `git config --list --system` | to view (may need sudo) |
| `git config --list --system \| grep editor` | to view default editor |
| `git config --edit --system` | to edit system config file |


### Global level

Stored in `$HOME/.gitconfig`

| Command | Description |
| ------- | ----------- |
| `git config --list --global` | to view |


### Repository level

Stored in `<repo_root>/.git/config`

| Command | Description |
| ------- | ----------- |
| `git config --list --local` | to view |
| `git config --local user.name [username]` | Set user name used in repository |
| `git config --local user.email [email]` | Set email used in repository |
