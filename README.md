# Fork of Boblightd for OSX

This is a fork of  Boblightd from https://github.com/arvydas/boblight

NOTE: This is work in progress with the objective of running the standard boblightd on OSX driving WS2812B via Arduino

From the source readme :-

### OSX

Prepare the build environment

	brew install autoconf automake libtool libusb git

Clone this repository

	git clone http://github.com/jaymonkey/boblight

Change directory

  cd boblight
	
Run the following commands to set up build environment and build boblight

	./autogen.sh
	./configure --without-x11 --without-portaudio
	make
	
Set up your configuration file as described in the [Boblight wiki](https://code.google.com/p/boblight/wiki/boblightconf). .

Run boblightd by issuing the following command

	./src/boblightd

Alternatively you can supply your own config file manually, for example

	./src/boblightd -c ./conf/custom.conf

