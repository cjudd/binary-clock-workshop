# Raspberry Pi Setup


## Install Raspbian Operating System

NOTE: Depends on [Raspbian Stretch Lite](http://director.downloads.raspberrypi.org/raspbian_lite/images/raspbian_lite-2018-06-29/2018-06-27-raspbian-stretch-lite.zip) and [Etcher](https://etcher.io).

1. Insert Micro SD card into SD card adapter and then insert SD card adapter into the SD card reader on your computer.
1. Launch Etcher.
1. Select downloaded Raspbian image.
1. Ensure the SD card reader drive is selected.
1. Flash the Micro SD card.

On Mac:

Follow https://desertbot.io/blog/ssh-into-pi-zero-over-usb.

On Windows:

Follow https://desertbot.io/blog/headless-pi-zero-ssh-access-over-usb-windows

## Configure Raspberry Pi

1. Move Micro SD card to Raspberry Pi Micro SD card slot.
1. Connect Raspberry Pi's USB port (not PWR) to computer using Micro USB to USB cable.
1. SSH to Raspbery Pi
    * Mac or Linux
        1. Open terminal window.
        1. SSH
        ```
        ssh pi@raspberrypi.local
        ```
        1. Approve authenticity of host.
1. Enter raspberry as password.

