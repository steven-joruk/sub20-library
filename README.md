This repository is based on xdimax's tar release [here](http://www.xdimax.com/sub20/sub20.html). Consider using [akiselev's python interface to the library](https://github.com/akiselev/PySub20).

## Set Up

### Ubuntu 16.04

1. Install the libusb development package: `sudo apt install libusb-1.0-0-dev`.
1. Set permissions via udev: `echo "SUBSYSTEM==\"usb\", ATTR{idVendor}==\"04d8\", ATTR{idProduct}==\"ffc3\", ACTION==\"add\", MODE=\"0666\"" | sudo tee /etc/udev/rules.d/65-sub-20.rules`
