Home: [ubuntu-setup](README.md)

# Adjust keyboard shortcuts for workspaces 

Following commands are for my favourite keyboard shortcuts. You can adapt it to your needs easily.
```bash
gsettings set org.gnome.desktop.wm.keybindings switch-to-workspace-down "['<Alt>Down']"
gsettings set org.gnome.desktop.wm.keybindings switch-to-workspace-up "['<Alt>Up']"
gsettings set org.gnome.desktop.wm.keybindings switch-to-workspace-left "['<Alt>Left']"
gsettings set org.gnome.desktop.wm.keybindings switch-to-workspace-right "['<Alt>Right']"

gsettings set org.gnome.desktop.wm.keybindings move-to-workspace-right "['<Ctrl><Alt>Right']"
gsettings set org.gnome.desktop.wm.keybindings move-to-workspace-left "['<Ctrl><Alt>Left']"
gsettings set org.gnome.desktop.wm.keybindings move-to-workspace-up "['<Ctrl><Alt>Up']"
gsettings set org.gnome.desktop.wm.keybindings move-to-workspace-down "['<Ctrl><Alt>Down']"
```

__Source:__ https://kubos.cz/2018/07/19/ubuntu-18-workspaces-grid