# linux-arch-installation
Linux Arch Installation using archfi
1. Download the ISO Arch from (according your country):
https://www.archlinux.org/download/
2. Make a bootable usb (you can uses rufus) for phisical machine, or use the iso direct with Oracle Virtual Box.
3. If phisical machine, make sure disable secure boot mode.
4. Reboot your machine with the ISO.
5. Make sure you have internet connection.
6. Code as follow in terminal
ping google.com    (use control+C  to quit from ping)
wifi-menu   (enter your credentials)
wget archfi.sf.net/archfi
7. At this time you will have blue screen.
Language -- English
Set Keyboard Layout -- us
Editor -- nano
Disk Partitions -- gpt
back (using tab or arrows)
Select Partitions and Install
  boot /dev/sda1
  swap /dev/sda2
  root /dev/sda3
  home /dev/sda4
Format Devices
  boot ext2
  swap swap
  root btrfs
Back or cancel
Mount
  Intall Arch Linux -- linux lts
  
  
  
