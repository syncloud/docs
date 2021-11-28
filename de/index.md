```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Über](https://github.com/syncloud/docs)

[en](https://github.com/syncloud/platform/wiki) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/index.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/index.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/index.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/index.md) | 

# Start

Das Erstellen von Syncloud-Geräten ist einfach. Sie benötigen: ARM- oder x64-Computer, Netzteil, Ethernet-Kabel, Festplatte oder SD-Karte. Sie benötigen auch einen Computer, um eine Boot-Festplatte oder SD-Karte zu erstellen. Folgen Sie einfach der Anleitung unten.

Weitere Informationen finden Sie auf den Wiki-Seiten [ganz unten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten). 

### Image herunterladen

Hier ist die Liste der unterstützten Boards und Links zu Image Dateien: 

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

### Image erstellen

1. Mit dem [Etcher Image Writer](https://www.balena.io/etcher/) ein Image auf eine Festplatte und/oder SD-Karte schreiben

Seien Sie vorsichtig und trennen Sie andere externe Laufwerke, bevor Sie schreiben, damit Sie nicht versehentlich alles löschen.

2. Legen Sie die Festplatte und/oder SD-Karte in das Gerät ein und starten Sie es.

Ihr Syncloud-Gerät ist bereit. Folgen Sie [dieser Anweisung](https://syncloud.org/setup.html), um es zu aktivieren. 

## Seiten

* [Benutzerkonten](https://github.com/syncloud/docs/blob/master/de/content/Accounts.md)
* [App Zugang](https://github.com/syncloud/docs/blob/master/de/content/App-access.md)
* [App Kanäle](https://github.com/syncloud/docs/blob/master/de/content/App-Channels.md)
* [Anleitung zur App-Portierung ](https://github.com/syncloud/docs/blob/master/de/content/App-porting-guide.md)
* [Backup](https://github.com/syncloud/docs/blob/master/de/content/Backup.md)
* [Backup SD-Karte](https://github.com/syncloud/docs/blob/master/de/content/Backup-SD-Card.md)
* [Bitwarden](https://github.com/syncloud/docs/blob/master/de/content/Bitwarden.md)
* [Booten von SATA](https://github.com/syncloud/docs/blob/master/de/content/Boot-from-SATA.md)
* [Browser Warnung (Zertifikat Problem)](https://github.com/syncloud/docs/blob/master/de/content/Browser-warning-(certificate-problem).md)
* [Custom Zertifikat](https://github.com/syncloud/docs/blob/master/de/content/Custom-certificate.md)
* [Custom Domain](https://github.com/syncloud/docs/blob/master/de/content/Custom-domain.md)
* [Geräteaktivierung](https://github.com/syncloud/docs/blob/master/de/content/Device-activation.md)
* [Device Migration](https://github.com/syncloud/docs/blob/master/de/content/Device-migration.md)
* [Diaspora](https://github.com/syncloud/docs/blob/master/de/content/Diaspora.md)
* [Docker](https://github.com/syncloud/docs/blob/master/de/content/Docker.md)
* [eMMC](https://github.com/syncloud/docs/blob/master/de/content/eMMC.md)
* [Externer Zugang](https://github.com/syncloud/docs/blob/master/de/content/External-access.md)
* [Externe Festplatte](https://github.com/syncloud/docs/blob/master/de/content/External-Disk.md)
* [FAQ](https://github.com/syncloud/docs/blob/master/de/content/FAQ.md)
* [Installer](https://github.com/syncloud/docs/blob/master/de/content/Installer.md)
* [Mail](https://github.com/syncloud/docs/blob/master/de/content/Mail.md)
* [Managed Domain](https://github.com/syncloud/docs/blob/master/de/content/Managed-domain.md)
* [Mehrere Festplatten](https://github.com/syncloud/docs/blob/master/de/content/Multiple-Disks.md)
* [Nextcloud](https://github.com/syncloud/docs/blob/master/de/content/Nextcloud.md)
* [PC](https://github.com/syncloud/docs/blob/master/de/content/PC.md)
* [Performance](https://github.com/syncloud/docs/blob/master/de/content/Performance.md)
* [Plex](https://github.com/syncloud/docs/blob/master/de/content/Plex.md)
* [Dateien Fernzugriff](https://github.com/syncloud/docs/blob/master/de/content/Remote-file-access.md)
* [Probleme berichten](https://github.com/syncloud/docs/blob/master/de/content/Report-problems.md)
* [Zu langsam](https://github.com/syncloud/docs/blob/master/de/content/Slow.md)
* [SSH](https://github.com/syncloud/docs/blob/master/de/content/SSH.md)
* [Syncloud-Mobile-App](https://github.com/syncloud/docs/blob/master/de/content/Syncloud-Mobile-App.md)
* [Wissenswertes vor dem Kauf eines Gerätes](https://github.com/syncloud/docs/blob/master/de/content/Things-to-know-before-buying-a-device.md)
* [Zeit](https://github.com/syncloud/docs/blob/master/de/content/Time.md)
* [Zugriff auf Gerät aus lokalem Netzwerk nicht möglich](https://github.com/syncloud/docs/blob/master/de/content/Unable-to-access-device-from-local-network.md)
* [Upgrade](https://github.com/syncloud/docs/blob/master/de/content/Upgrade.md)
* [Users](https://github.com/syncloud/docs/blob/master/de/content/Users.md)
* [Virtual-Box](https://github.com/syncloud/docs/blob/master/de/content/Virtual-Box.md)
* [VPN](https://github.com/syncloud/docs/blob/master/de/content/VPN.md)
