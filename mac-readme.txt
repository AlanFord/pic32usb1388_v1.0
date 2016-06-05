Prerequisites for a clean compile

Install Autoconf. For instructions see http://mac-dev-env.patrickbougie.com/autoconf/

Change to the ./hidapi/hidapi directory and then:
./autoconf
./make

Change to the ./libusb-1.0.9/libusb-1.0.9 directory and then:
./autoconf
./make

To compile, use this command:
gcc -o pic32usb main.c ./hidapi/hidapi/mac/.libs/libhidapi.a ./libusb-1.0.9/libusb-1.0.9/libusb/.libs/libusb-1.0.a -framework CoreFoundation -framework IOKit
