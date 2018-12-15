Pacdrive
==============

Command line utility for Ultimarc PacDrive board.

#### Introduction:
This utility is a more specific implementation of the Ultimac-Linux project. This utility targets only the Ultimarc PacDrive board. 

If you need support for other Ultimarc boards, please look at the the Ultimarc-linux project by Katie-Snow.

#### Required Libraries
To build this tool the following libraries need to be install on your system.
* autoreconf
* automake
* libudev-dev
* json-c (0.11), <a href='https://github.com/json-c/json-c/wiki'>site</a>
* libusb-1.0 (1.0.18), <a href='http://libusb.info'>site</a>
* libtool

#### UDEV Rule:
This utility requires folder permission changes to the usb device directories before it can do the configuration changes to the boards.  The udev rule in the base directory named 21-ultimarc.rules needs to be placed in /etc/udev/rules.d directory.  Placing the file in that directory usually requires root permissions.

#### Building Utility:
To build this project, at the base directory run the following commands
* ./autogen.sh
* ./configure
* make

If you need extra debug statements for the IPac boards then run the following
* ./configure CFLAGS='-DDEBUG'
* make

The executable will be in src/umtool directory and named pacdrive.
* ./pacdrive 1 3 5 7 9 11 13 14   
Turns on every other output by connecting it to ground.

