Home: [ubuntu-setup](README.md)

# Force alt + tab to switch only on current workspace

Open _dconf-editor_, go to **/org/gnome/shell/app-switcher** and set **current-workspace-only**.

If you don't have installer _dconf-editor_ you can install it by running following command.
```bash
sudo apt install dconf-editor
```

__Source:__ https://askubuntu.com/questions/464946/force-alt-tab-to-switch-only-on-current-workspace-in-gnome-shell