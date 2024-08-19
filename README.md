# Lab Computer Setup

* [ECEN 224](ecen224.md)
* [ECEN 220/320](ecen320.md)
* [ECEN 330](ecen330.md)
* ECEN 390: same as [ECEN 330](ecen330.md)
* [ECEN 423/323](ecen423.md)
* [ECEN 426](ecen426.md)
* [ECEN 427](ecen427.md)
* [ECEN 522R - Security](ecen522r_security/requirements.md)

Other non-class related setup needs:
* [F4PGA](f4pga.md)

## Other apt packages
```
sudo apt install \
    vim \
    tmux \
    screen \
    wget \
    htop \
    minicom \
    zsh \
    python3.10-venv
```

## Permissions to Serial Devices

Add a file: `/etc/udev/rules.d/50-myusb.rules` with contents:
```
KERNEL=="ttyACM[0-9]*",MODE="0666"
KERNEL=="ttyUSB[0-9]*",MODE="0666"
```

Add these lines as well for SD card imaging permissions:
 ```
 KERNEL=="sd*", SUBSYSTEMS=="usb", MODE="0666"
 ```
