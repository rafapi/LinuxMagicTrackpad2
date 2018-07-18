# LinuxMagicTrackpad2

- I am using mtrack as the Xorg driver here because it provides a lot more input granularity.

## Installing

- This has been tested on Arch Linux running a 4.16.13-2 kernel.

- Both the Linux-Magic-Trackpad-2-Driver and xf86-input-mtrack need to be installed.

- `Linux-Magic-Trackpad-2-Drive` should be installed by running `install.sh` from the scripts folder. This will take care of building and installing the driver. `Note that we need the Dynamic Kernel Module Support framework (`dkms`) installed on the system to run that script.`

- `xf86-input-mtrack` needs to be installed as follows:

```
./configure --prefix=/usr
make
make install
```

## Configuration

- Place the config file from the examples folder into ```/etc/X11/xorg.conf.d``` and restart the X session (```sudo systemctl restart lightdm.service```)
