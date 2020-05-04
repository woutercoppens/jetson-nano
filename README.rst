# jetson-nano
Setup files for my jetson nano

First boot after deploying sdcard:

sudo apt-get update

sudo apt-get upgrade

To disable GUI on boot, run:

sudo systemctl set-default multi-user.target
To enable GUI again issue the command:

sudo systemctl set-default graphical.target
to start Gui session on a system without a current GUI just execute:

sudo systemctl start gdm3.service

sudo apt-get install avahi-daemon screen tmux 
sudo apt-get install docker-compose
sudo usermod -aG docker wouter

cleanup:
sudo apt remove --purge libreoffice* -y

sudo apt autoremove

sudo cp 45-allow-colord.pkla /etc/polkit-1/localauthority/50-local.d/

xrdp (to figure out once):
sudo adduser xrdp ssl-cert
