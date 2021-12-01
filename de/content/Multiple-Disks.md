```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Multiple-Disks) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Multiple-Disks.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Multiple-Disks.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Multiple-Disks.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Multiple-Disks.md) | 

# Mehrere Festplatten

### Geräte

Derzeit verkaufen wir keine vorkonfigurierten Multi-Disk-Geräte.

Aber es gibt viele Optionen auf dem Markt (arm, amd64), hier eine Liste mit relativ günstigen Beispielen:

* Helios 4/64 (https://wiki.kobol.io/helios4/syncloud/)
* Shuttle XH270, 4 Festplatten (Barebone)
* Shuttle XH110V, 2 Festplatten (Barebone)
* Asus VM65N, 2 Festplatten (nicht Barebone)
* Gigabyte BRIX Gaming BNi7HG4-950 (barebpne)
* Viele Intel NUK unterstützen mehrere Festplatten (Barebone)

### RAID

Lesen Sie diese Dokumentation, um ein RAID zu erstellen: https://wiki.kobol.io/helios4/mdadm

1. Erstellen Sie eine einzelne Partitionstabelle auf der RAID-Festplatte
2. Formatieren Sie die Partition mit dem ext4-Dateisystem
3. Stellen Sie sicher, dass es nicht montiert ist
4. Schaltfläche „Speicherformat“ nicht verwenden
5. Aktivieren: Einstellungen - Speicher aktivieren

### Richtige Unterstützung der Syncloud-Benutzeroberfläche

Problem: https://github.com/syncloud/platform/issues/571
