# Hackintosh-ASUS-Flying-fortress-FXPRO-GL552VW
这可以帮助您完美地运行macOS High Sierra & Mojave & Catalina（最高10.15.5 - 19F101）  
您也可以使用它运行macOS 10.15.5或更高版本

This can help you run macOS High Sierra & Mojave & Catalina(10.15.5 - 19F101 maximum)perfectly.  
You can also use it to run macOS 10.15.5 or higher future version,but the sound card driver may not work on these versions.

## 注意 & Attention
想要用这个EFI启动你的macOS，你需要做这几件事：  
  1.把你的UEFI固件版本升级为304版本  
  2.在UEFI设置中关闭Fast Boot, CSM Mode, Secure Boot  
  3.在UEFI中的Graphic Configuration菜单中把dvmt设置为256mb  
少了以上任意一条，你都无法启动系统或者某些驱动有问题  

To start your macOS with this EFI, you need to do a few things:  
   1. Upgrade your UEFI Firmware to version 304  
   2. Turn off Fast Boot, CSM Mode, Secure Boot in the UEFI settings  
   3. Set dvmt to 256mb in the Graphic Configuration menu in the UEFI  
Without any of the above, you cannot start the system or there are problems with some drivers  

## 联系我 & Contact me
__如果你有问题，可以在百度贴吧联系我（YJHuaa）或给我发邮件jonesbak@outlook.com 如果你在某个黑苹果群遇见我也可以直接问我，昵称一般是Elton__  
__If you have problems, contact me with jonesbak@outlook.com__

## 关于转载 & About repost  
该项目仅供技术交流，请勿用于商业用途，转载请注明来源及原作者，请尊重我的劳动，谢谢！  
This project is only for technical communicating, please do not use it for commercial purposes, please indicate the source and original author for reprint, please respect my labor, thank you!

## 电脑配置 & The hardware configuration of my laptop

Hardware | Detail
---------|----------
CPU      | Intel Core i5-6300HQ
IGPU     | HD530
EGPU     | Nvidia Geforce GTX960M(4G)
Wifi     | Boradcom 94350(DW1820A)
SSD      | SAMSUNG MZNLF128HCHP-00004
RAM      | SK HYNIX 8G*1 2133MHz
Display	 | AUO TN 1080P
TouchPad | ELAN 1000
Sound    | Conexant 20751/2

该项目包括Clover v5.0 r5118（支持macOS Catalina）  
我将启动等待时间设置成了2秒，如果你想用这个配置来安装macOS，你可能需要进入clover界面后，按“o”键，然后在boot-args中添加“-v”，这样你就可以获得详细的错误信息

This project includes clover v5.0 r5118.(macOS Catalina Supported)  
I set the clover to wait for 2 second before booting automatically. If you want to use it for installing macOS,you may need to
press the "o" key after entering the clover interface,and then add "-v" in boot args so that you can get detailed error information.

## 显卡 & Graphics GPU
由于硬件问题和新版本macOS中缺乏驱动程序支持，macOS Mojave & Catalina不支持Nvidia GPU，此配置中我禁用了独立显卡

据我们所知，macOS Catalina和Mojave没有Nvidia显卡的驱动程序，因此您只能在这些系统上使用核显

如果要使用Nvidia显卡，你只能使用macOS High Sierra及以下版本，然后配置NVIDIA Webdriver

* [Nvidia WebDriver 下载](https://www.tonymacx86.com/Nvidia-drivers/)

注意：你可以尝试驱动GTX960m显卡，但是据我所知，clover不支持这款显卡的Optimus技术，所以未必有用  

-----------------------------------------------------------------------------------

The Nvidia GPU is not supported because of hardware differences and lack of driver support in the new version macOS.   

As far as we know, NVIDIA GPU do not have drivers to support them on macOS Catalina & Mojave, so you can only
use IGPU on these systems. 

If you want to use EGPU, you can only use macOS High Sierra and below,and then configure NVIDIA Webdriver.

* [Nvidia WebDriver Download](https://www.tonymacx86.com/nvidia-drivers/)

Note: You can try to drive the GTX960m graphics card, but as far as I know, clover does not support Optimus technology for this graphics card, so it may not work

## 声卡问题 & Sound card issues
经过我多次研究发现，重启后可能出现声卡失效的问题是由于Windows系统重新启动时不能重置HDA导致的，目前无解，等我有空会发布该机型的opencore引导即可解决该问题  

After many studies, I found that the problem of sound card failure after restarting is due to the fact that the HDA cannot be reset when the Windows system reboot. There is no solution at present. When I have time, I will release the Opencore Bootloader of the model to solve the problem.
