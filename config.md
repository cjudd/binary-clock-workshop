# Configure

During this lab, you connect the Raspberry Pi to your computer so you can remotely login using the monitor on your comuputer rather then having to attach an external monitor, keyboard and mouse. Finally you will configure your Raspberry Pi to synchronize it's clock with the internet so it aways has the correct time. 

## Connect to Raspberry Pi

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
    * Windows
        1. Open Putty
        1. Enter raspberrypi.local into Host Name and press the Open button.
        1. Approve authentication of host.
        1. Enter login of pi and press enter.
1. Enter **raspberry** as password.

NOTE: If you get a **WARNING: POSSIBLE DNS SPOOFING DETECTED!** error run the following command and try sshing again.

```
ssh-keygen -R raspberrypi.local
```

## Configure Networking & Timezone

Networking and Timezone should be configured so it can automatically get the correct time.

NOTE: When you bring the binary clock home or change WiFi networks, you will have to reconfigure the network.

1. At the Raspberry Pi's command-line type:
```
sudo raspi-config
```
1. Goto Network Options.
1. Choose Wi-fi.
1. Enter codemash for SSID and press enter for passphrase.
1. Goto Localisation Options.
1. Choose Change Timezone.
1. US
1. Select Eastern or timezone you reside in.
1. Finish.
1. Type the following on the command-line to validate date and time.
```
date
```

NOTE: While you are in raspi-config, it is probably a good idea to change the password as the default password is insecure and well known!!!

## Manually Configure Time

If WiFi isn't available, you can set the current time using this command.

```
sudo date -s "09 JAN 2020 19:11:00"
```

---

[NEXT](basic_hardware.md)