```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Backup-SD-Card) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Backup-SD-Card.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Backup-SD-Card.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Backup-SD-Card.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Backup-SD-Card.md) | 

# Backup SD-Karte

## Manuelle Sicherung

Es ist nicht sicher, ein Backup auf einem laufenden Gerät zu erstellen, daher wird empfohlen, es auszuschalten und die SD-Karte mit einem PC zu verbinden.

### Etcher

Etcher unterstützt noch keine Backup-Funktion, überprüfen Sie den Status: https://github.com/resin-io/etcher/issues/266

### dd (Linux, Mac)

```
dd if=/dev/mmcblk01 of=/data/backup.img bs=1M
```

### Win32 Disk-Imager (Windows)

https://sourceforge.net/projects/win32diskimager/
