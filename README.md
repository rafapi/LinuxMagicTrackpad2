# LinuxMagicTrackpad2

## Installing

- This has been tested on Arch Linux running a 4.16.13-2 kernel.

- Both the Linux-Magic-Trackpad-2-Driver and xf86-input-mtrack need to be installed. The first one works fine using the install.sh script from the scripts folder.

- The xf86 package needs to be installed as follows:

``` ./configure --prefix=/usr
make
make install
```

## Configuration

- Place the config file from the examples folder into ```/etc/X11/xorg.conf.d``` and restart the X session (```sudo systemctl restart lightdm.service```)
