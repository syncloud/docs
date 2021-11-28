```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Custom-domain) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Custom-domain.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Custom-domain.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Custom-domain.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Custom-domain.md) | 

# Eigene Domain

Wenn Sie unseren Domain-Service (syncloud.it) nicht nutzen möchten, können Sie das Gerät mit Ihrer eigenen benutzerdefinierten Domain aktivieren.

Sie verlieren eine Option zum Aktualisieren der dinamyc-IP-Adresse (syncloud.it-Funktion). Ansonsten gibt es keine Einschränkung bei Gerät oder Apps.

### DNS Server

Wenn Sie eine eigene Domain haben, stellen Sie sicher, dass Ihr DNS-Server über die richtigen Einträge verfügt:

```
A [IPv4]-Beispiel.com
AAAA [IPv6] example.com
CNAME *.example.com example.com
```

Die zweite Zeile ist ein Wildcard-Eintrag. Bei einigen DNS-Anbietern können Sie einfach die Wildcard-Funktion für Ihre Domain aktivieren.

## IPv4

Es sollte einer von diesen sein:

* Geräte-IP Wenn Ihr Gerät eine öffentliche IP hat
* Router-IP (öffentliche IP-Adresse vom ISP anfordern, die Sie nicht haben). Erstellen Sie entsprechende Portzuordnungen zu Ihrem Gerät.

## IPv6

DNS sollte auf die Geräte-IP verweisen, da IPv6 immer öffentlich ist.

### Hosts-Datei (nur wenn Sie keinen DNS-Server haben)

In diesem Abschnitt geht es um die Hosts-Datei auf jedem Client-PC, mit dem Sie auf das Syncloud-Gerät zugreifen.

Hosts-Datei auf einem Gerät sollte unberührt bleiben.

Wenn Sie keinen DNS-Server haben und Syncloud in Ihrem LAN ausprobieren möchten, bearbeiten Sie Ihre Hosts-Datei:

```
[Öffentliche IP] example.com (Gerät selbst)
[Öffentliche IP] [app].example.com (Zeile pro App)
```

Linux: /etc/hosts

Windows: c:\System32\drivers\etc\hosts

### Portzuordnungen

Wenn Sie keine öffentliche IP auf Ihrem Gerät haben, sollten Sie die IP Ihres Routers verwenden und die Portweiterleitung auf Ihr Gerät einstellen:

```
80 -> [Geräte-IP]:80
443 -> [Geräte-IP]:443
```

#### Dynamische IP-Adresse

In vielen Fällen stellt Ihr Internetanbieter Ihrem Router/Modem standardmäßig eine dynamische öffentliche IP-Adresse zur Verfügung, die sich täglich oder so ändert.

In diesem Fall möchten Sie vielleicht eine statische öffentliche IP-Adresse kaufen, die sich nie von Ihrem Internetanbieter ändert.

Eine andere Möglichkeit besteht darin, Ihren DNS-Anbieter zu überprüfen, ob er eine Möglichkeit hat, Ihre IP jeden Tag zu aktualisieren. Viele DNS-Anbieter haben diese Funktion. In diesem Fall müssen Sie alle 10 Minuten einen einfachen Befehl auf Ihrem Gerät ausführen (sie sollten weitere Informationen bereitstellen).

#### Let's Encrypt Zertifikat

Gerät sollte nur dann automatisch ein echtes Zertifikat erhalten, wenn Port 80 aus dem Internet sichtbar ist (siehe Port-Mapping oben)

### Aktivieren Sie Ihr Gerät

Greifen Sie mit der IP-Adresse auf Ihr Gerät zu oder verwenden Sie die Android Syncloud-App.

Aktivieren Sie mit Ihrer benutzerdefinierten Domain.
