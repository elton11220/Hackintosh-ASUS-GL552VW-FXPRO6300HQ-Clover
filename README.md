# Hackintosh-ASUS-Flying-fortress-FXPRO-GL552VW
This can help you run macOS High Sierra & Mojave & Catalina(10.15.3 maximum)perfectly.  
You can also use it to run macOS 10.15.4 or higher future version,but the sound card driver may not work on these versions.


Here is my configuration of my laptop

Hardware | Detail 
---------| -------
CPU      | Intel Core i5-6300HQ
IGPU     | HD530
EGPU     | Nvidia Geforce GTX960M(4G)
Wifi     | Boradcom 94350(DW1820A)
SSD      | SAMSUNG MZNLF128HCHP-00004
RAM      | SK HYNIX 8G*1 2133MHz
Display	 | AUO TN 1080P
TouchPad | ELAN 1000
Sound	   | Conexant 20751/2

This project includes clover v5109.  
I set the clover to wait for 1 second before booting automatically. If you want to use it for installing macOS,you may need to
press the "o" key after entering the clover interface,and then add "-v" in boot args so that you can get detailed error information.

## 显卡 & Graphics GPU
由于硬件差异和新版本macOS中缺乏驱动程序支持，不支持Nvidia GPU  
>（此配置中禁用它是为了节省电源）

据我们所知，macOS Catalina和Mojave没有Nvidia显卡的驱动程序，因此您只能在这些系统上使用核显

如果要使用Nvidia显卡，只能使用macOS High Sierra及以下版本，然后配置NVIDIA Webdriver

*[Nvidia WebDriver下载]（https://www.tonymacx86.com/Nvidia-drivers/）

-----------------------------------------------------------------------------------

The Nvidia GPU is not supported due to hardware differences and lack of driver support in the new version macOS.   
>(It is disabled in this configuration to save power)

As far as we know, NVIDIA graphics cards do not have drivers to support them on macOS Catalina & Mojave, so you can only
use IGPU on these systems. 

If you want to use EGPU, you can only use macOS High Sierra and below,and then configure NVIDIA Webdriver.

* [Nvidia WebDriver Download](https://www.tonymacx86.com/nvidia-drivers/)

## 联系我 & Contact me
__如果你有问题，可以在百度贴吧联系我（YJHuaa）或给我发邮件joensbak@outlok.com__
__If you have problems, contact me with jonesbak@outlook.com__
