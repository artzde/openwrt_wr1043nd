Flash Factory image for Routers Running TP-LINK Firmware
A common failure is due to the fact that the user is connected to another network while upgrading firmware as a result an incomplete copy gets loaded into the router.
So follow the steps while upgrading to third party firmware
    - Make sure your computer is connected to the router only via Ethernet Cable, do not be connected to multiple networks including wireless.
    - Make sure power supply is not disconnected and Ethernet Cable is not loose.

If you lose the connection while uploading the firmware the only way is to recover using Serial Console and tftp
http://wiki.openwrt.org/toh/tp-link/tl-wr1043nd#recovery.via.serial.console

Flash Sysupgrade image for Routers Running Older OpenWRT Firmware
    - Upgrading between OpenWRT is safer as the image is downloaded to the Router and verified before flashing.

Use the Sysupgrade back to factory to revert to factory firmware, if you cannot use the webinterface, 
you need to ssh into the router scp the file into /tmp directory and run sysupgrade with override switches.