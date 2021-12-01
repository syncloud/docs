```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Time) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Time.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Time.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Time.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Time.md) | 

# Zeit

Manchmal können Uhrzeit und Datum des Geräts nicht mehr synchron sein.

Bitte führen Sie diese Befehle mit SSH (https://github.com/syncloud/platform/wiki/SSH) aus, um zu sehen, ob das Problem behoben ist:

```
service ntp stop
ntpd -gq
Dienst ntp starten
```
