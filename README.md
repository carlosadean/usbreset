# usbreset
This simple application simulates the plug/unplug of a usb device

### How to compile?
$ gcc -o usbreset usbreset.c

### How to use it?
Get the Bus and Device ID of the USB device you want to reset:

$ lsusb  
Bus **001** Device **008**: ID 0ac8:3420 Z-Star Microelectronics Corp. Venus USB2.0 Camera

### Execute the program with sudo privileges
Make necessary substitution for `<Bus>` and `<Device>` ids as found by running the lsusb command:

$ sudo  ./usbreset  /dev/bus/usb/**002**/**003**


font: http://askubuntu.com/questions/645/how-do-you-reset-a-usb-device-from-the-command-line
