1. Configure the USB driver for our board:
        
    * Copy the `99-ftdi-sio.rules` file to `/etc/udev/rules.d/` directory.
    * Run `sudo udevadm control --reload-rules` to reload the rules.
    * Reboot the machine

1. Install the following packages:

        sudo apt-get install -y gcc make gcc-avr avr-libc avrdude
