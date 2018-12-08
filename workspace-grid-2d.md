Home: [ubuntu-setup](README.md)

# Workspace grid (2D)

If you miss 2D workspace grid from Ubuntu 16.

## Installation
Easyies way is by switching toggle on [this page](https://extensions.gnome.org/extension/484/workspace-grid/). But firstly we have to install **chrome-gnome-shell**:
```bash
sudo apt install chrome-gnome-shell
```

## Name workspaces
Open _dconf-editor_ and go to **/org/gnome/desktop/wm/preferences/workspace-names**. Write names in **Custom value** field as array of strings (example: `['Name1', 'Name2]`). Changes will be applied after restarting Ubuntu.

If you don't have installer _dconf-editor_ you can install it by running following command.
```bash
sudo apt install dconf-editor
```


__Source:__ https://github.com/zakkak/workspace-grid