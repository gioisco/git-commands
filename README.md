Git Commands to become a pro
============
_Great git commands for improve your skills ...and that sometimes I forget_

### Daily commands
| Command | Description |
| ------- | ----------- |
|`git add . -p`| allows to stage piece of code |
|`git stash show -p` | show diff in last stash|
|`git stash show -p stash@{1}` | show diff in stash@{1}|
|`git checkout -- <file>`| WARNING revert the `<file>` in working directory. It is distructive command |

### Basic Configuration
#### System level

| Command | Description |
| ------- | ----------- |
| `git config --list --system` | to view (may need sudo) |
| `git config --list --system \| grep editor` | to view default editor |
| `git config --edit --system` | to edit system config file |


#### Global level

| Command | Description |
| ------- | ----------- |
| `git config --list --global` | to view |


#### Repository level

| Command | Description |
| ------- | ----------- |
| `git config --list --local` | to view |
| `git config --local user.name [username]` | Set user name used in repository |
| `git config --local user.email [email]` | Set email used in repository |
