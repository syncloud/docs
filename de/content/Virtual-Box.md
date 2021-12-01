```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Virtual-Box) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Virtual-Box.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Virtual-Box.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Virtual-Box.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Virtual-Box.md) | 

# Virtual Box

1. Virtuelle Box installieren
2. Extrahieren Sie die Datei syncloud-vbox-[version].vdi.xz in syncloud-vbox-[version].vdi
3. Erweitern Sie die Festplatte (Standard ist nur 3 GB). Dadurch erhalten Sie 50 GB.

```
VBoxManage modifymedium disk syncloud-amd64-[version].vdi --resize 50000
```

4. VM basierend auf Debian x64 erstellen

5. Verwenden Sie die vorhandene virtuelle Festplatte und wählen Sie die extrahierte vdi-Datei aus

6. [Optional] Einstellungen -> Netzwerk -> Adapter 1: An "Bridged Adapter" anhängen

     Dadurch kann sich die VM auf einer separaten IP in Ihrem Netzwerk befinden, sodass sie Portzuordnungen durchführen und für eine Telefonerkennung sichtbar ist.

7. Start

8. Aktivieren durch Öffnen der VM-IP-Adresse im Browser

9. Erweitern Sie die Bootdiskette in den Einstellungen - Interner Speicher
