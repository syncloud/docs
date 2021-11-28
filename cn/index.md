```diff
! 翻译正在开发中。 请依赖英文的原始版本。
```

[关于](https://github.com/syncloud/docs)

[en](https://github.com/syncloud/platform/wiki) | 
[de](https://github.com/syncloud/docs/blob/master/de/index.md) | 
cn | 
[ru](https://github.com/syncloud/docs/blob/master/ru/index.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/index.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/index.md) | 

# 开始

构建 Syncloud 设备很容易。 您将需要：ARM 或 x64 计算机、电源适配器、以太网电缆、磁盘或 SD 卡。 您还需要一台计算机来创建启动盘或 SD 卡。 只需按照以下说明操作即可。

可以在右侧的 wiki 页面上找到更多信息。

### 下载图片

以下是支持的电路板列表和图像文件链接： 


|Board Name|Syncloud Image|
|:---|:---|
|[Banana Pi M1](https://www.banana-pi.org/)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-bananapim1-21.10.img.xz)|
|[Banana Pi M1+](https://www.banana-pi.org/)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-bananapim1-21.10.img.xz)|
|[Banana Pi M2](https://www.banana-pi.org/)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-bananapim2-21.10.img.xz)|
|[Banana Pi M3](https://www.banana-pi.org/)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-bananapim3-21.10.img.xz)|
|[Cubieboard](cubieboard.org)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-cubieboard-21.10.img.xz)|
|[Cubieboard 2](cubieboard.org)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-cubieboard2-21.10.img.xz)|
|[Cubietruck](cubieboard.org)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-cubietruck-21.10.img.xz)|
|[BeagleBone Black](http://beagleboard.org/Products/BeagleBone+Black)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-beagleboneblack-21.10.img.xz)|
|[Raspberry Pi 2 (B)](http://www.raspberrypi.org/)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-beagleboneblack-21.10.img.xz)|
|[Raspberry Pi 3/4 (B/B+, 4G/8G)](http://www.raspberrypi.org/)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-raspberrypi-21.10.img.xz)|
|[Odroid C2](https://www.hardkernel.com/shop/odroid-c2)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-c2-21.10.img.xz)|
|[Odroid XU3](https://www.hardkernel.com/shop/odroid-xu3)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-21.10.img.xz)|
|[Odroid HC1](https://www.hardkernel.com/shop/odroid-hc1-home-cloud-one)|[SD](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-sd-21.10.img.xz), [SATA](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-21.10.img.xz), [info](https://github.com/syncloud/docs/blob/master/cn/content/Boot-from-SATA.md)|
|[Odroid HC2](https://www.hardkernel.com/shop/odroid-hc2-home-cloud-two)|[SD](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-sd-21.10.img.xz), [SATA](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-21.10.img.xz), [info](https://github.com/syncloud/docs/blob/master/cn/content/Boot-from-SATA.md)|
|[Odroid HC4](https://www.hardkernel.com/shop/odroid-hc4)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-hc4-21.10.img.xz)|
|[Odroid XU4](https://www.hardkernel.com/shop/odroid-xu4-special-price)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-21.10.img.xz)|
|[Odroid N2](https://www.hardkernel.com/shop/odroid-n2-with-4gbyte-ram)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-n2-21.10.img.xz)|
|[Odroid U3](https://www.hardkernel.com/shop/odroid-u3)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-u3-21.10.img.xz)|
|[Tinker](https://www.asus.com/uk/Single-Board-Computer/Tinker-Board)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-tinker-21.10.img.xz)|
|[Helios4](http://kobol.io/helios4)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-helios4-21.10.img.xz)|
|[Helios64](http://kobol.io/helios64)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-helios64-21.10.img.xz)|
|[Rock64](https://www.pine64.org/)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-rock64-21.10.img.xz)|
|x64 [Virtual Box](https://www.virtualbox.org/wiki/Downloads)|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-amd64-21.10.vdi.xz), [info](https://github.com/syncloud/docs/blob/master/cn/content/Virtual-Box.md)|
|x64 Linux [Docker](https://www.docker.com/)|[info](https://github.com/syncloud/docs/blob/master/cn/content/Docker.md)|
|x64 Syncloud OS [Legacy BIOS]|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-amd64-21.10.img.xz), [info](https://github.com/syncloud/docs/blob/master/cn/content/PC.md)|
|x64 Syncloud OS [UEFI] recommended for NUC or any other Intel/AMD system|[下载](https://github.com/syncloud/platform/releases/download/21.10/syncloud-amd64-uefi-21.10.img.xz), [info](https://github.com/syncloud/docs/blob/master/cn/content/PC.md)|

### 写图像

1. 使用 Etcher 图像写入器将图像写入磁盘和/或 SD 卡

在写入之前请小心并分离其他外部驱动器，以免意外擦除其中的所有内容。

2. 将磁盘和/或 SD 卡插入设备并启动它。

您的 Syncloud 设备已准备就绪。 按照此说明激活它。

## 页面

* [Accounts](https://github.com/syncloud/docs/blob/master/cn/content/Accounts.md)
* [App-access](https://github.com/syncloud/docs/blob/master/cn/content/App-access.md)
* [App-Channels](https://github.com/syncloud/docs/blob/master/cn/content/App-Channels.md)
* [App-porting-guide](https://github.com/syncloud/docs/blob/master/cn/content/App-porting-guide.md)
* [Backup](https://github.com/syncloud/docs/blob/master/cn/content/Backup.md)
* [Backup-SD-Card](https://github.com/syncloud/docs/blob/master/cn/content/Backup-SD-Card.md)
* [Bitwarden](https://github.com/syncloud/docs/blob/master/cn/content/Bitwarden.md)
* [Boot-from-SATA](https://github.com/syncloud/docs/blob/master/cn/content/Boot-from-SATA.md)
* [Browser-warning-(certificate-problem)](https://github.com/syncloud/docs/blob/master/cn/content/Browser-warning-(certificate-problem).md)
* [Custom-certificate](https://github.com/syncloud/docs/blob/master/cn/content/Custom-certificate.md)
* [Custom-domain](https://github.com/syncloud/docs/blob/master/cn/content/Custom-domain.md)
* [Device-activation](https://github.com/syncloud/docs/blob/master/cn/content/Device-activation.md)
* [Device-migration](https://github.com/syncloud/docs/blob/master/cn/content/Device-migration.md)
* [Diaspora](https://github.com/syncloud/docs/blob/master/cn/content/Diaspora.md)
* [Docker](https://github.com/syncloud/docs/blob/master/cn/content/Docker.md)
* [eMMC](https://github.com/syncloud/docs/blob/master/cn/content/eMMC.md)
* [External-access](https://github.com/syncloud/docs/blob/master/cn/content/External-access.md)
* [External-Disk](https://github.com/syncloud/docs/blob/master/cn/content/External-Disk.md)
* [FAQ](https://github.com/syncloud/docs/blob/master/cn/content/FAQ.md)
* [Installer](https://github.com/syncloud/docs/blob/master/cn/content/Installer.md)
* [Mail](https://github.com/syncloud/docs/blob/master/cn/content/Mail.md)
* [Managed-domain](https://github.com/syncloud/docs/blob/master/cn/content/Managed-domain.md)
* [Multiple-Disks](https://github.com/syncloud/docs/blob/master/cn/content/Multiple-Disks.md)
* [Nextcloud](https://github.com/syncloud/docs/blob/master/cn/content/Nextcloud.md)
* [PC](https://github.com/syncloud/docs/blob/master/cn/content/PC.md)
* [Performance](https://github.com/syncloud/docs/blob/master/cn/content/Performance.md)
* [Plex](https://github.com/syncloud/docs/blob/master/cn/content/Plex.md)
* [Remote-file-access](https://github.com/syncloud/docs/blob/master/cn/content/Remote-file-access.md)
* [Report-problems](https://github.com/syncloud/docs/blob/master/cn/content/Report-problems.md)
* [Slow](https://github.com/syncloud/docs/blob/master/cn/content/Slow.md)
* [SSH](https://github.com/syncloud/docs/blob/master/cn/content/SSH.md)
* [Syncloud-Mobile-App](https://github.com/syncloud/docs/blob/master/cn/content/Syncloud-Mobile-App.md)
* [Things-to-know-before-buying-a-device](https://github.com/syncloud/docs/blob/master/cn/content/Things-to-know-before-buying-a-device.md)
* [Time](https://github.com/syncloud/docs/blob/master/cn/content/Time.md)
* [Unable-to-access-device-from-local-network](https://github.com/syncloud/docs/blob/master/cn/content/Unable-to-access-device-from-local-network.md)
* [Upgrade](https://github.com/syncloud/docs/blob/master/cn/content/Upgrade.md)
* [Users](https://github.com/syncloud/docs/blob/master/cn/content/Users.md)
* [Virtual-Box](https://github.com/syncloud/docs/blob/master/cn/content/Virtual-Box.md)
* [VPN](https://github.com/syncloud/docs/blob/master/cn/content/VPN.md)
