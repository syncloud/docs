```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Boot-from-SATA) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Boot-from-SATA.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Boot-from-SATA.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Boot-from-SATA.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Boot-from-SATA.md) | 

# *insert page name here*

**WARNUNG**: Sie müssen dies nicht tun, wenn Sie ein Gerät bei uns kaufen, es ist alles fertig und getestet.

### SD-Karte

Einige Boards wie Odroid HC1/HC2 haben einen SATA-Steckplatz. Leider kann man davon nicht direkt booten und im Moment keine SD-Karte verwenden.

Die Problemumgehung besteht darin, ein spezielles SD-Image auf eine SD-Karte und ein SATA-Image auf eine SATA-Festplatte zu schreiben. Auf diese Weise bleiben alle betriebssystembezogenen Dateien und Apps selbst auf der SATA-Festplatte.

Sie müssen die SD-Karte weiterhin eingesteckt lassen, da sie zum Laden des Kernels beim Booten verwendet wird.

### Größe

Standardmäßig beträgt die Bildgröße 3 GB. Um das Dateisystem auf die tatsächliche Festplattengröße zu erweitern, verwenden Sie Einstellungen - Speicher - Boot erweitern, bevor Sie eine App installieren.

Wenn die Festplatte immer noch 3 GB anzeigt, führen Sie diesen Befehl aus:

```
/snap/platform/current/bin/boot_extend.sh
```
