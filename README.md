# linux-arch-installation
Linux Arch Installation using archfi
1. Download the ISO Arch from (according your country):
https://www.archlinux.org/download/
2. Make a bootable usb (you can uses rufus) for phisical machine, or use the iso direct with Oracle Virtual Box.
3. If phisical machine, make sure disable secure boot mode.
4. Reboot your machine with the ISO.
5. Make sure you have internet connection.
6. Code as follow in terminal
7. ping google.com    (use control+C  to quit from ping)
8. wifi-menu   (enter your credentials)
9. wget archfi.sf.net/archfi
10. sh archfi
# At this time you will have the archfi blue screen.
1. Language -- English
2. Set Keyboard Layout -- us
3. Editor -- nano
4. Disk Partitions -- gpt
5. back (using tab or arrows)
6. Select Partitions and Install
7.  boot /dev/sda1
8.  swap /dev/sda2
9.  root /dev/sda3
10.  home /dev/sda4
11. Format Devices
12.  boot ext2
13.  swap swap
14.  root btrfs
15. Back or cancel
16. Mount
17.  Intall Arch Linux -- linux lts
    
  
  
