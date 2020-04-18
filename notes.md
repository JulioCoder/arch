# Packages

#### After bare bones installation

`yay -S git xterm rxvt-unicode terminator awesome ttf-roboto rofi compton i3lock xclip flameshot gnome-keyring qt5-styleplugins-git htop xorg-xbacklight nautilus materia-gtk-theme`

#### Utilities

`yay -S nautilus`
`yay -S materia-gtk-theme`

`wget -qO- https://git.io/papirus-icon-theme-install | sh`

#### Material-Awesome Config

`sudo systemctl disable lxdm`

`sudo systemctl enable lightdm`

`yay -S lightdm-slick-greeter`

`sudo vim /etc/lightdm/lightdm.conf`

> greeter-session=lightdm-slick-greeter

Search: **Customize Look and Feel** to change appearance

> In Widget set Materia-Dark-compact
> In Icon Theme set Papirus

#### Some commands to remember

`sudo pacman -S <some_pkgs>`

`sudo pacman -Rnsd <some_pkg>`

`sudo pacman -Rnsd $(pacman -Qtdq)`

`mkdir -p ~/large/path/`

`rxvt-unicode`

#### Markdown Cheat Sheet

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
