# Hackintosh-ASUS-Flying-fortress-FXPRO-GL552VW
Hackintosh Clover configurations for Asus Flying Fortress FX-PRO(i5-6300HQ HD530 Version)


This can help you run macOS High Sierra & Mojave & Catalina（10.15.3 maximum） perfectly.

You can also use it to run macOS 10.15.4 or higher future version,but the sound card driver may not work on these versions.


Here is my configuration of my laptop

Hardware | Detail 
---------| -------
CPU      | Intel Core i5-6300HQ
IGPU     | HD530
EGPU     | Nvidia Geforce GTX960M
Wifi     | Boradcom 94350(DW1820a)
SSD      | SAMSUNG MZNLF128HCHP-00004
RAM      | SK HYNIX 8G*1 2133MHz
Display	 | AUO TN 1080P
TouchPad | ELAN 1000
Sound	   | Conexant 20751/2

This project includes clover(r5109).I set the clover to wait for 1 second before booting automatically. If you want to use it
for installing macOS,you may need to press the "o" key after entering the clover interface,and then add "-v" in boot args so
that you can get detailed error information.

# Graphics GPU
The Nvidia GPU is not supported due to hardware differences and lack of driver support in the new version macOS. 

It is disabled in this configuration to save power.

As far as we know, NVIDIA graphics cards do not have drivers to support them on macOS Catalina & Mojave, so you can only
use IGPU on these systems. If you want to use EGPU, you can only use macOS High Sierra and below,and then configure NVIDIA Webdriver.

* [Nvidia WebDriver Download](https://www.tonymacx86.com/nvidia-drivers/)
