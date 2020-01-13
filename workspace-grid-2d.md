Home: [ubuntu-setup](README.md)

# Workspace grid (2D)

If you miss 2D workspace grid from Ubuntu 16.

## Installation
Easyies way is by switching toggle on [this page](https://extensions.gnome.org/extension/484/workspace-grid/). But firstly we have to install **chrome-gnome-shell**:
```bash
sudo apt install chrome-gnome-shell
```

If you want more than 4 workspaces (default count) you have to install ```gnome-tweaks``` to be able to set custom count.
```bash
sudo apt install gnome-tweaks
```
Then launch _Tweaks_ and go to the _Workspaces_ section. Select _Static Workspaces_ instead of _Dynamic Workspaces_ and set the _Number of Workspaces_ to your preferred one, 6 for example.

![Tweaks menu](https://i.stack.imgur.com/6Wbng.png)

## Name workspaces
Open _dconf-editor_ and go to **/org/gnome/desktop/wm/preferences/workspace-names**. Write names in **Custom value** field as array of strings (example: `['Name1', 'Name2]`). Changes will be applied after restarting Ubuntu.

If you don't have installer _dconf-editor_ you can install it by running following command.
```bash
sudo apt install dconf-editor
```


__Sources:__ 
https://github.com/zakkak/workspace-grid
https://askubuntu.com/questions/1081251/multiple-workspaces-on-ubuntu-18-04-1-lts-and-later-with-gnome-shell