/ [ubuntu-setup](README.md) / workspace-grid-2d

# Workspace grid (2D)

If you miss 2D workspace grid from Ubuntu 16.

## Installation
Easyies way is by sitching toggle on this page - https://extensions.gnome.org/extension/484/workspace-grid/
But firstly we have to install **chrome-gnome-shell**:
```bash
sudo apt install chrome-gnome-shell
```

## Name workspaces
Install _dconf-editor_:
```bash
sudo apt install dconf-editor
```
Open it and go to _/org/gnome/desktop/wm/preferences/workspace-names_. Write names in _Custom value_ field as array of strings (example: `['Name1', 'Name2]`). Changes will be applied after restaning Ubuntu.

__Source:__ https://github.com/zakkak/workspace-grid