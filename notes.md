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

#### Skip Grub Menu

`sudo nano /etc/default/grub`
> Change GRUB_TIMEOUT from 5 to 0
`sudo grub-mkconfig -o /boot/grub/grub.cfg`

#### Some commands to remember

Linux failing at Start `Control + Alt + F2`

When Stock in VIM

`Control + Q`

`sudo pacman -S <some_pkgs>`

`sudo pacman -Rnsd <some_pkg>`

`sudo pacman -Rnsd $(pacman -Qtdq)`

`mkdir -p ~/large/path/`

`rxvt-unicode`

`sshfs usuario@your_ip:/ ~/test -C -p 9876`

Network Manager `nmcli`
`nmcli device show`
`ip route`
`lsblk -f`

create `git init --bare`

remove `rm -rf HEAD config hooks objects branches description info refs`

#### Awesome

Mod + Ctl + j : focus on next screen
Mod + o : move windows to other screen


#### Markdown Cheat Sheet

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

#### djando-server

after terminate and start django-server
update PUBLICK IP in django_project/settings.py
`sudo service apache2 restart`
