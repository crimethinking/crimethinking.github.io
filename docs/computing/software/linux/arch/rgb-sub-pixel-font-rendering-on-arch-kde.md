# RGB sub-pixel font rendering on Arch + KDE
Fonts on KDE on Arch after installation look off to my eyes compared to Kubuntu; turns out by default RGB
sub-pixel font rendering is not enabled. Changing the sub-pixel rendering settings in KDE System Settings
does not work, but `fontconfig` preset symlinking does:
``` sh
sudo ln -s /usr/share/fontconfig/conf.avail/10-sub-pixel-rgb.conf /etc/fonts/conf.d
```
Reboot
