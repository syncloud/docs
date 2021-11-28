```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Device-activation) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Device-activation.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Device-activation.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Device-activation.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Device-activation.md) | 

# Geräteaktivierung

Möglichkeiten zur Aktivierung:

1. Die Android/iPhone Syncloud-App sollte Ihr Gerät erkennen können, wenn es mit demselben WLAN-Netzwerk verbunden ist.

2. Die Browseraktivierung ist eine alternative Möglichkeit, indem Sie die IP Ihres Geräts auf Ihrer Routerseite nachschlagen und diese URL in Ihrem Browser öffnen: https://[Geräte-IP].

Sie benötigen ein Konto bei https://syncloud.it für unseren Domainnamen oder Sie können Ihren eigenen Domainnamen verwenden.

Außerdem müssen Sie Ihre Geräteanmeldeinformationen zuweisen, um Ihr Gerät zu schützen.

Wenn dies nicht funktioniert, müssen Sie die Netzwerkverbindung oder die Korrektheit des Bildes überprüfen.

Überprüfen Sie [Probleme melden]()

### Gerätepasswort vergessen

Es gibt zwei Möglichkeiten, das Gerät zurückzusetzen:

* Deaktivieren Sie das Gerät, indem Sie die folgende Datei auf der Hauptfestplatte entfernen:
```
/var/snap/platform/current/platform.db
```
* Schreiben Sie das Geräte-Image erneut.
