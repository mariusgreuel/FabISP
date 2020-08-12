# FabISP, a fab-able in-system programmer

This is a fork of the [FabISP firmware](http://fab.cba.mit.edu/content/archive/projects/fabisp/) by David A. Mellis, which is based on USBtiny by Dick Streefland.

The goal of this fork is to add support for WinUSB to FabISP firmware to eliminate the need for third-party USB drivers in Windows, such as libusb0.

In this firmware, a [Microsoft OS feature descriptor](https://docs.microsoft.com/en-us/windows-hardware/drivers/usbcon/microsoft-defined-usb-descriptors) and WinUSB compatibility descriptor was added. When a USB device with this firmware is plugged in, Windows will automatically load the built-in WinUSB driver.

In order to use the FabISP/USBtiny with WinUSB support, you also need tools that support WinUSB, such as [AVRDUDE for Windows](https://github.com/mariusgreuel/avrdude).