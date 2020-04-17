# linux-arch-installation
Linux Arch Installation using archfi
1. Download the ISO Arch from (according your country):
https://www.archlinux.org/download/
2. Make a bootable usb (you can uses rufus) for phisical machine, or use the iso direct with Oracle Virtual Box.
3. If phisical machine, make sure disable secure boot mode.
4. Reboot your machine with the ISO.
5. Make sure you have internet connection.
6. Code as follow in terminal
7.      ping google.com    (use control+C  to quit from ping)
8.      wifi-menu   (enter your credentials)
9.      pacman -Sy    
10.     wget archfi.sf.net/archfi
11.     sh archfi
# At this time you will have the archfi blue screen.
1. Language -- English
2. Set Keyboard Layout -- us
3. Editor -- nano
4. Disk Partitions -- gpt
5. back (using tab or arrows)
6. Select Partitions and Install
7. boot /dev/sda1
8. swap /dev/sda2
9. root /dev/sda3
10. home /dev/sda4
11. Format Devices
12. boot ext2
13. swap swap
14. root btrfs
15. Back or cancel
16. Mount
17. Intall Arch Linux -- linux lts    (this takes several minutes)
18. Config Arch Linux
19. Set Computer Name
20. Keyboard Layout -- us
21. Set Locale -- en_US
22. Set Time --  US
23. Set root password
24. Generate fstab -- UUID
25. Bootloader -- grub -- install grub
26. Install bootloader
27. Back
28. Enable dhcpcd
29. Archdi -- yes
30. Install and Run Archdi
31. sourceforge
32. Updates
33. Install pacman-contrib
34. Install yay
35.	Upgrade with yay
36. Back
37. Install
38. Console Generic
39. Default + add (tab key to select, then OK)
        [X]neofetch   
40. Compression Tools (all)
41. Networks Toos -- Default and add 
        [X]nmap & [X]speedtest
42. Back
__________
43. System
44. Services -- default selection is OK -- then all yes
45. File System -- default selection and add
        [X]sshfs [X]difs [X]gvfs
46. Sound -- default selection is OK
47. Back
__________
48. XORG
49. Gpu Infos -- OK
50. Install -- default is OK
51. Fonts -- default -- ok
52. TTF -- optional
53. Input Drivers -- dfault is OK
54. Back
# Desktop Enviroment (example, according what you want)
1. Desktop Environment LXDE-GTK3
2. Apllication -- Internet -- chromium
3. Dev -- code
4. Systerm -- gparted
Back
1. Config
2. Bash -- editor.sh -- nano
3. alias.sh -- default is ok
4. ps1.sh -- minimal -- yes
5. Update -- yes -- yes
6. Back
# Accounts
1. Add User -- your name
2. Sudoers -- add sudoer -- OK
3. Back.
# Systemd
4. Systemd -- timedatectl
5. Enable timedatectl -- ok
6. Edit /etc/systemd/timesyncd.conf (modify as follows)
        Before: #NTP=             After: NTP=us.pool.ntp.org
        Before: #Fallback(etc...) After: Fallback(etc...)
        Save the file: control+o then Enter then control+x
7. Back
8. Back
9. Back
10. Exit
11. Back
12. Umount
13. Back
14. Reboot
15. Yes
# Ready Arch - Bare Bones

## Some pkgs to install

`yay -S awesome rofi compton i3lock xclip flameshot gnome-keyring qt5-styleplugins-git ttf-rototo htop rofi`