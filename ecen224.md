1. Install Ubuntu 22

2. Install packages
```
sudo apt update

sudo apt install \
  rpi-imager
```

3. Install VS Code <https://code.visualstudio.com/>

4. Add a file: `/etc/udev/rules.d/99-diskaccess.rules` with contents:
```
SUBSYSTEM=="block", SUBSYSTEMS=="usb", ATTRS{idVendor}=="*", ATTRS{idProduct}=="*", KERNEL=="sda*", GROUP="diskaccess", MODE="0660"
```

5. Create a group named `diskaccess` and ...?
