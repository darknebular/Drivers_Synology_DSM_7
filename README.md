##  Drivers_Synology_DSM_7
# Drivers for Wi-Fi dongles, DTVs USB dongles, etc. For Synology DSM 7

These files enable to have USB Dongles, like Wi-Fi, DTV, etc. for your Synology DSM 7.

Choose your arquitecture, and put them in /lib/modules in your NAS.
To view your arquitecture ([help](https://kb.synology.com/es-es/DSM/tutorial/What_kind_of_CPU_does_my_NAS_have))

Then you must to run via SSH these commands:

`sudo -i`

`/sbin/modprobe usbserial`

`/sbin/modprobe ftdi_sio`

`/sbin/modprobe cdc-acm`

`chmod 777 /dev/ttyUSB0`

`chmod 777 /dev/ttyACM0`

`sudo ./lib/modules/start-usb-drivers.sh`




# ¡¡ENJOY!!
