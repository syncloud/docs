```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/External-Disk) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/External-Disk.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/External-Disk.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/External-Disk.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/External-Disk.md) | 

# Externe Festplatte

### Externe Festplatte aktivieren

Syncloud ermöglicht es Ihnen, zusätzliche externe Festplatten (USB oder SATA) für die Datenspeicherung in Ihren Apps zu aktivieren.

Unterstütztes Dateisystem mit einer Partition: ext4.

Dies kann in Einstellungen - Speicher erfolgen.

Warnung: Ihre vorhandenen Dateien werden bei der Aktivierung nicht von der internen/externen Festplatte verschoben.

### Datenpfade

Interner Speicher: /opt/disk/internal

Externer Speicher: /opt/disk/external

Aktiver Datenträger: /data (Link zu einem der oben genannten)

### Externe Festplatte formatieren

Sie können auch eine externe Festplatte initialisieren, um sie kompatibel zu machen, aber dadurch werden alle Daten darauf gelöscht.
