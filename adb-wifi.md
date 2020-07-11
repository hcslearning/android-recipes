ADB WIFI
=========

See here: http://forum.xda-developers.com/showpost.php?p=7594419&postcount=9

Connect device via USB and make sure debugging is working.

adb tcpip 5555
adb connect <DEVICE_IP_ADDRESS>:5555

Disconnect USB and proceed with wireless debugging.
adb -s <DEVICE_IP_ADDRESS>:5555 usb to switch back when done.

No root required!
To find the IP address of the device: run adb shell and then netcfg. You'll see it there.
