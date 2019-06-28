# Desktop Performance Widget Conky customized for Raspberry Pi 
I simplified an existing guide by pre-creating the additional required files and updating the install steps to use them.  
Based on this post by Novaspirit.com https://www.novaspirit.com/2017/02/23/desktop-widget-raspberry-pi-using-conky/ 
Conky created by Brenden Matthews which can be found https://github.com/brndnmtthws/conky

We first start by installing Conky
```
sudo apt-get -y install conky
```

Download the pre-made custom layout config file
> If you want to add/remove/change anything have a look at all the settings here http://conky.sourceforge.net/config_settings.html
```
sudo wget -O /home/pi/.conkyrc https://raw.githubusercontent.com/frankpintosr/rpi_conky/master/rpi3_conkyrc
```

Download the shell script
```
sudo wget -O /usr/bin/conky.sh https://raw.githubusercontent.com/frankpintosr/rpi_conky/master/conky.sh
```

Download the file to add Conky to desktop and autostart
```
sudo wget -O /etc/xdg/autostart/conky.desktop https://raw.githubusercontent.com/frankpintosr/rpi_conky/master/conky.desktop
```

After a reboot you will see the widget added to your desktop!
```
sudo reboot now
```

