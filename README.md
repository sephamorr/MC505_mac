MC505_mac
=========

A few tools for working with the MC505 FPGA Board on osx: patch for urjtag, fxload for mac (to use with Xilinx Platform Cable)

1: There is a patch for compiling urjtag on mac. Requires libusb1.0, installed from homebrew. Based on urjtag svn r2040.
	The requisite bdsl converted files are included in the patch for this board.

2: FXLoad for mac, a few modernity updates from https://github.com/nall/nexys2-osx/tree/master/fxload (previously not updated since 2009)
	Firmwares for the Xilinx Platform Cable are included in the xpc_firmware folder
	xpcload is a oneliner shell script to upload the firmware to the usb device. Upon uploading, the programmer will reenumate as a xpc and can be then used (device ID changes from 0x000D to 0x0008)