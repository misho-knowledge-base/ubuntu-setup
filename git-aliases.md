Home: [ubuntu-setup](README.md)

# Git aliases

Some useful Git aliases:

```bash
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.c commit
git config --global alias.alias "! git config --get-regexp ^alias\. | sed -e s/^alias\.// -e s/\ /\ =\ /"
git config --global alias.update "pull --rebase"
git config --global alias.lg "log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(cyan)<%an>%Creset' --abbrev-commit --date=relative"
```