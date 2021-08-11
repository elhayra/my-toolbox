## Install Manjaro
- install manjaro-kde-plasma [here](https://manjaro.org/download/)
- right after installation, update the mirrors list and priorities faster mirrors, and update the system:
`sudo pacman-mirrors --fasttrack && sudo pacman -Syyu`
- backup the system by using [clonezilla](https://www.youtube.com/watch?v=EW4_tqBaczw)
- customize the desktop to [your liking](https://www.youtube.com/watch?v=exQh0_JKBJQ)
- install other tools, login to accounts and then backup again


## Installing Nvidia Drivers
Go through [this guide](https://www.addictivetips.com/ubuntu-linux-tips/nvidia-graphics-drivers-manjaro/) :
- first install Manjaro settings manager
`sudo pacman -S manjaro-settings-manager`

- open the settings manager by running:
`manjaro-settings-manager`

- go to hardware, right click on nvidia and 'install'. be patiant. after installation is done, reboot

- if some of the windows text and fonts looks zoomed or strange, go through this [guide](https://archived.forum.manjaro.org/t/after-installing-proprietary-nvidia-driver-some-programs-are-scaled-too-big/150439/11) :

force DPI to the /etc/X11/mhwd.d/nvidia.conf in the Section "Monitor"
Option "DPI" "96 x 96"

or maybe use

Option              "UseEdidDpi" "False"
Option              "DPI" "96 x 96"

But pay attention to where the EndSection is for Section "Monitor" and put the lines right above EndSection ...
Reboot after that.




