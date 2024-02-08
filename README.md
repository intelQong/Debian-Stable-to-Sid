# Debian stable to sid/unstable instructions

## Steps :
1) Go to [Debian website](https://www.debian.org/) and download netinst.iso file
2) Make a USB stick bootable using [Balena](https://etcher.balena.io/) or [Ventoy](https://www.ventoy.net/en/index.html)
3) Go to UFEI Boot menu and select your live usb.
4) Start installing
5) After installation completion, open the terminal
6) Type `su` and enter root password
7) now enter `nano /etc/apt/sources.list`
8) Comment out everything and enter `###### Debian Main sid repos #####
deb http://deb.debian.org/debian/ unstable main contrib non-free-firmware
deb-src http://deb.debian.org/debian/ unstable main contrib non-free-firmware` ( you can find the txt file [here](sources.list) )
9) Save using **CTRL + O** and Enter
10) Exit using **CTRL + X**
11) now do `apt update`
12) and `apt full-upgrade`


