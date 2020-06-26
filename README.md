General info. 
More in depth info will have its own file.

Remove extra boot options from UEFI boot up
https://superuser.com/questions/930725/how-to-delete-os-from-boot-menu

No wifi after OS installation? Use phone plugged in as a USB tether. 
Try updating OS first. Otherwise, follow STA / bcmwl-kernel-source install instructions
https://help.ubuntu.com/community/WifiDocs/Driver/bcm43xx
Then I needed to add those 2 commands to the startup programs list. For some reason, need to run after each reboot.

Commonly used programs:
1. telegram
2. pycharm
3. gitkraken
4. speedcrunch (add to system settings > shortcuts, ctrl+shift+z)
5. nvim
6. qbit
7. peppermint
8. unified remote

gnome tweaks:
2. firefox extension for extensions.gnome.org
dashtodock
audio switcher
panel osd
clock override (%Y.%m.%d | %H:%M)

cascadia code font
microsoft fonts: sudo apt search ttf-mscorefonts-installer

exfat protoshare access:
https://itsfoss.com/mount-exfat/

logitech mx master mouse driver (enables middle click)
(has own folder)

Southwest Flight Auto Check-in
https://github.com/pyro2927/SouthwestCheckin
(has own folder)

xbox one controller wireless driver
https://github.com/medusalix/xow
Don't forget to hit the "pair" button on the top side of the xbox controller, not just the stupid xbox button on the front.
(has own folder)

Set default audio device on reboot:
https://askubuntu.com/questions/1038490/how-do-you-set-a-default-audio-output-device-in-ubuntu-18-04
use pactl list short sinks #this shows audio sources
in /etc/pulse/default.pa, change the last lines to:
set-default-sink alsa_output.pci-0000_00_1b.0.analog-stereo
#set-default-source input
and then comment out the load-module module-switch-on-connect line.
