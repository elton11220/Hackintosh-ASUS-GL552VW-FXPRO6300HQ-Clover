# Hackintosh-ASUS-Flying-fortress-FXPRO-GL552VW
这可以帮助您完美地运行macOS High Sierra & Mojave & Catalina（最高10.15.3）  
您也可以使用它运行macOS 10.15.4或更高版本，但声卡驱动程序可能无法在这些版本上运行

This can help you run macOS High Sierra & Mojave & Catalina(10.15.3 maximum)perfectly.  
You can also use it to run macOS 10.15.4 or higher future version,but the sound card driver may not work on these versions.


#### Here is my configuration of my laptop

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

该项目包括Clover 5109版本（支持macOS Catalina）  
我将启动等待时间设置成了1秒，如果你想用这个配置来安装macOS，你可能需要进入clover界面后，按“o”键，然后在boot-args中添加“-v”，这样你就可以获得详细的错误信息

This project includes clover v5109.(macOS Catalina Supported)  
I set the clover to wait for 1 second before booting automatically. If you want to use it for installing macOS,you may need to
press the "o" key after entering the clover interface,and then add "-v" in boot args so that you can get detailed error information.

## 显卡 & Graphics GPU
由于硬件问题和新版本macOS中缺乏驱动程序支持，macOS Mojave & Catalina不支持Nvidia GPU，此配置中我禁用了独立显卡

据我们所知，macOS Catalina和Mojave没有Nvidia显卡的驱动程序，因此您只能在这些系统上使用核显

如果要使用Nvidia显卡，你只能使用macOS High Sierra及以下版本，然后配置NVIDIA Webdriver

* [Nvidia WebDriver 下载](https://www.tonymacx86.com/Nvidia-drivers/)

-----------------------------------------------------------------------------------

The Nvidia GPU is not supported because of hardware differences and lack of driver support in the new version macOS.   

As far as we know, NVIDIA GPU do not have drivers to support them on macOS Catalina & Mojave, so you can only
use IGPU on these systems. 

If you want to use EGPU, you can only use macOS High Sierra and below,and then configure NVIDIA Webdriver.

* [Nvidia WebDriver Download](https://www.tonymacx86.com/nvidia-drivers/)

## 联系我 & Contact me
__如果你有问题，可以在百度贴吧联系我（YJHuaa）或给我发邮件joensbak@outlook.com__  
__If you have problems, contact me with jonesbak@outlook.com__
