Home: [ubuntu-setup](README.md)

#  Adding Git branch name and some colors

Add these lines in your **~/.bashrc** file.

```bash
# Add git branch if its present to PS1
parse_git_branch() {
 git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/(\1)/'
}

# Bash console colors
RED="\[\033[0;31m\]"
YELLOW="\[\033[0;33m\]"
GREEN="\[\033[0;32m\]"
NO_COLOR="\[\033[0m\]"

# Console format and colors
#PS1="$GREEN\u@\h$NO_COLOR:\w$YELLOW \$(parse_git_branch)$NO_COLOR\$ "
PS1="\[\e]0;\u@\h: \w\a\]${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]$YELLOW \$(parse_git_branch)$NO_COLOR\$ "

# Alases per directory
export PROMPT_COMMAND='if [[ "$bashrc" != "$PWD" && "$PWD" != "$HOME" && -e .bashrc ]]; then bashrc="$PWD"; . .bashrc; fi'
```
