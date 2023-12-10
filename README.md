# Git commands to become a Pro

Great git commands to improve your skills... and sometimes you might forget!


## Daily commands

| Command | Description |
| ------- | ----------- |
|`git add . -p`| allows to stage piece of code |
|`git stash show -p` | show diff in last stash|
|`git stash show -p stash@{1}` | show diff in stash@{1}|
|`git checkout -- <file>`| WARNING revert the `<file>` in working directory. It is distructive command |


## Git Configuration

When using `git config`, you can specify three levels of configuration:

| Level         | Description                                              |
| ------------- | -------------------------------------------------------- |
| `--system`    | System-wide configuration stored in `/etc/gitconfig`. Requires sudo permissions for modification. |
| `--global`    | User-specific configuration stored in `$HOME/.gitconfig`. |
| `--local`     | Repository-specific configuration stored in `<repo_root>/.git/config`. |


## Show config

Usually you have only user (`--global`) and repo (`--local`) configuration. Use this modifier to restrict what do you want to see.

Try with `git config --system -l` to check the system level configuration exists.

| Command | Description |
| ------- | ----------- |
| `git config --list ` | or with `-l` show ALL configuration varibles |
| `git config -l --system  ` | show configuration varibles at system level (may need sudo) |
| `git config -l --global ` | show configuration varibles at user level |
| `git config -l --local ` | show configuration varibles at repo level |
| `git config -l --global \| grep editor` | to view default editor |

## Set config

### Initial configuration

Set your `user.name` and `user.email` for local repository

| Command | Description |
| -------------------------------------------- | --------------- |
| `git config --local user.name <username>`    | Set user name used in repository |
| `git config --local user.email <email>`      | Set email used in repository |

Or for global purposes:

| Command | Description |
| -------------------------------------------- | --------------- |
| `git config --global user.name <username>`   | Set user name used everywere |
| `git config --global user.email <email>`     | Set email used everywere |


To store the password permanently and set the editor:

| Command | Description |
| -------------------------------------------- | --------------- |
| `git config --local credential.helper store` | Store password permanently for repository |
| `git config --global core.editor vim`        | Set vim editor for system |

Edit properties manually:

| Command | Description |
| ------- | ----------- |
| `git config --edit --system` | Edit the system configuration file |


#### Custom Configuration

| Task              | Command                                | Description                                      |
| ----------------- | -------------------------------------- | ------------------------------------------------ |
| Create Git Alias  | `git config --global alias.s 'status'` | Add the alias `s` to call `git status` using `git s` (also with autocomplete) |

