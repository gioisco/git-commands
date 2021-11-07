Git Commands to become a pro
============
_Great git commands for improve your skills ...and that sometimes I forget_

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
