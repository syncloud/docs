```diff
! Перевод находится в стадии разработки. Пожалуйста, полагайтесь на оригинальную версию на английском языке.
```

[О](https://github.com/syncloud/docs)

[en](https://github.com/syncloud/platform/wiki) | 
[de](https://github.com/syncloud/docs/blob/master/de/index.md) | 
[cn](https://github.com/syncloud/docs/blob/master/cn/index.md) | 
ru | 
[fr](https://github.com/syncloud/docs/blob/master/fr/index.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/index.md) | 

# Начинать

Создать устройство Syncloud легко. Вам понадобится: компьютер ARM или x64, адаптер питания, кабель Ethernet, диск или SD-карта. Вам также понадобится компьютер для создания загрузочного диска или SD-карты. Просто следуйте инструкциям ниже.

Более подробную информацию можно найти на вики-страницах справа.

### Скачать изображение

Вот список поддерживаемых досок и ссылки на файлы изображений:


|Board Name|Syncloud Image|
|:---|:---|
|[Banana Pi M1](https://www.banana-pi.org/)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-bananapim1-21.10.img.xz)|
|[Banana Pi M1+](https://www.banana-pi.org/)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-bananapim1-21.10.img.xz)|
|[Banana Pi M2](https://www.banana-pi.org/)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-bananapim2-21.10.img.xz)|
|[Banana Pi M3](https://www.banana-pi.org/)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-bananapim3-21.10.img.xz)|
|[Cubieboard](cubieboard.org)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-cubieboard-21.10.img.xz)|
|[Cubieboard 2](cubieboard.org)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-cubieboard2-21.10.img.xz)|
|[Cubietruck](cubieboard.org)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-cubietruck-21.10.img.xz)|
|[BeagleBone Black](http://beagleboard.org/Products/BeagleBone+Black)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-beagleboneblack-21.10.img.xz)|
|[Raspberry Pi 2 (B)](http://www.raspberrypi.org/)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-beagleboneblack-21.10.img.xz)|
|[Raspberry Pi 3/4 (B/B+, 4G/8G)](http://www.raspberrypi.org/)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-raspberrypi-21.10.img.xz)|
|[Odroid C2](https://www.hardkernel.com/shop/odroid-c2)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-c2-21.10.img.xz)|
|[Odroid XU3](https://www.hardkernel.com/shop/odroid-xu3)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-21.10.img.xz)|
|[Odroid HC1](https://www.hardkernel.com/shop/odroid-hc1-home-cloud-one)|[SD](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-sd-21.10.img.xz), [SATA](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-21.10.img.xz), [info](https://github.com/syncloud/docs/blob/master/de/content/Boot-from-SATA.md)|
|[Odroid HC2](https://www.hardkernel.com/shop/odroid-hc2-home-cloud-two)|[SD](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-sd-21.10.img.xz), [SATA](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-21.10.img.xz), [info](https://github.com/syncloud/docs/blob/master/de/content/Boot-from-SATA.md)|
|[Odroid HC4](https://www.hardkernel.com/shop/odroid-hc4)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-hc4-21.10.img.xz)|
|[Odroid XU4](https://www.hardkernel.com/shop/odroid-xu4-special-price)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-xu3and4-21.10.img.xz)|
|[Odroid N2](https://www.hardkernel.com/shop/odroid-n2-with-4gbyte-ram)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-n2-21.10.img.xz)|
|[Odroid U3](https://www.hardkernel.com/shop/odroid-u3)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-odroid-u3-21.10.img.xz)|
|[Tinker](https://www.asus.com/uk/Single-Board-Computer/Tinker-Board)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-tinker-21.10.img.xz)|
|[Helios4](http://kobol.io/helios4)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-helios4-21.10.img.xz)|
|[Helios64](http://kobol.io/helios64)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-helios64-21.10.img.xz)|
|[Rock64](https://www.pine64.org/)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-rock64-21.10.img.xz)|
|x64 [Virtual Box](https://www.virtualbox.org/wiki/Downloads)|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-amd64-21.10.vdi.xz), [info](https://github.com/syncloud/docs/blob/master/de/content/Virtual-Box.md)|
|x64 Linux [Docker](https://www.docker.com/)|[info](https://github.com/syncloud/docs/blob/master/de/content/Docker.md)|
|x64 Syncloud OS [Legacy BIOS]|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-amd64-21.10.img.xz), [info](https://github.com/syncloud/docs/blob/master/de/content/PC.md)|
|x64 Syncloud OS [UEFI] recommended for NUC or any other Intel/AMD system|[Download](https://github.com/syncloud/platform/releases/download/21.10/syncloud-amd64-uefi-21.10.img.xz), [info](https://github.com/syncloud/docs/blob/master/de/content/PC.md)|

### Написать изображение

1. Запись образа на диск и / или SD-карту с помощью средства записи изображений Etcher

Будьте осторожны и отсоедините другие внешние диски перед записью, чтобы случайно не стереть с них все.

2. Вставьте диск и / или SD-карту в устройство и загрузите его.

Ваше устройство Syncloud готово. Следуйте этой инструкции, чтобы активировать его.

## Страницы

* [Accounts](https://github.com/syncloud/docs/blob/master/ru/content/Accounts.md)
* [App-access](https://github.com/syncloud/docs/blob/master/ru/content/App-access.md)
* [App-Channels](https://github.com/syncloud/docs/blob/master/ru/content/App-Channels.md)
* [App-porting-guide](https://github.com/syncloud/docs/blob/master/ru/content/App-porting-guide.md)
* [Backup](https://github.com/syncloud/docs/blob/master/ru/content/Backup.md)
* [Backup-SD-Card](https://github.com/syncloud/docs/blob/master/ru/content/Backup-SD-Card.md)
* [Bitwarden](https://github.com/syncloud/docs/blob/master/ru/content/Bitwarden.md)
* [Boot-from-SATA](https://github.com/syncloud/docs/blob/master/ru/content/Boot-from-SATA.md)
* [Browser-warning-(certificate-problem)](https://github.com/syncloud/docs/blob/master/ru/content/Browser-warning-(certificate-problem).md)
* [Custom-certificate](https://github.com/syncloud/docs/blob/master/ru/content/Custom-certificate.md)
* [Custom-domain](https://github.com/syncloud/docs/blob/master/ru/content/Custom-domain.md)
* [Device-activation](https://github.com/syncloud/docs/blob/master/ru/content/Device-activation.md)
* [Device-migration](https://github.com/syncloud/docs/blob/master/ru/content/Device-migration.md)
* [Diaspora](https://github.com/syncloud/docs/blob/master/ru/content/Diaspora.md)
* [Docker](https://github.com/syncloud/docs/blob/master/ru/content/Docker.md)
* [eMMC](https://github.com/syncloud/docs/blob/master/ru/content/eMMC.md)
* [External-access](https://github.com/syncloud/docs/blob/master/ru/content/External-access.md)
* [External-Disk](https://github.com/syncloud/docs/blob/master/ru/content/External-Disk.md)
* [FAQ](https://github.com/syncloud/docs/blob/master/ru/content/FAQ.md)
* [Installer](https://github.com/syncloud/docs/blob/master/ru/content/Installer.md)
* [Mail](https://github.com/syncloud/docs/blob/master/ru/content/Mail.md)
* [Managed-domain](https://github.com/syncloud/docs/blob/master/ru/content/Managed-domain.md)
* [Multiple-Disks](https://github.com/syncloud/docs/blob/master/ru/content/Multiple-Disks.md)
* [Nextcloud](https://github.com/syncloud/docs/blob/master/ru/content/Nextcloud.md)
* [PC](https://github.com/syncloud/docs/blob/master/ru/content/PC.md)
* [Performance](https://github.com/syncloud/docs/blob/master/ru/content/Performance.md)
* [Plex](https://github.com/syncloud/docs/blob/master/ru/content/Plex.md)
* [Remote-file-access](https://github.com/syncloud/docs/blob/master/ru/content/Remote-file-access.md)
* [Report-problems](https://github.com/syncloud/docs/blob/master/ru/content/Report-problems.md)
* [Slow](https://github.com/syncloud/docs/blob/master/ru/content/Slow.md)
* [SSH](https://github.com/syncloud/docs/blob/master/ru/content/SSH.md)
* [Syncloud-Mobile-App](https://github.com/syncloud/docs/blob/master/ru/content/Syncloud-Mobile-App.md)
* [Things-to-know-before-buying-a-device](https://github.com/syncloud/docs/blob/master/ru/content/Things-to-know-before-buying-a-device.md)
* [Time](https://github.com/syncloud/docs/blob/master/ru/content/Time.md)
* [Unable-to-access-device-from-local-network](https://github.com/syncloud/docs/blob/master/ru/content/Unable-to-access-device-from-local-network.md)
* [Upgrade](https://github.com/syncloud/docs/blob/master/ru/content/Upgrade.md)
* [Users](https://github.com/syncloud/docs/blob/master/ru/content/Users.md)
* [Virtual-Box](https://github.com/syncloud/docs/blob/master/ru/content/Virtual-Box.md)
* [VPN](https://github.com/syncloud/docs/blob/master/ru/content/VPN.md)
