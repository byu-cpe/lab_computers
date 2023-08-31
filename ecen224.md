1. Install Ubuntu 22

2. Install packages
```
sudo apt update

sudo apt install \
  rpi-imager
```

3. Install VS Code <https://code.visualstudio.com/>

4. Add a file: `/etc/udev/rules.d/50-myusb.rules` with contents:
```
KERNEL=="sd*", SUBSYSTEMS=="usb", MODE="0666"
```
