```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Unable-to-access-device-from-local-network) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Unable-to-access-device-from-local-network.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Unable-to-access-device-from-local-network.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Unable-to-access-device-from-local-network.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Unable-to-access-device-from-local-network.md) | 

# Zugriff auf Gerät aus lokalem Netzwerk nicht möglich

### Externer Zugriffsmodus ist deaktiviert

Die übliche Ursache dafür ist eine falsche oder langsame Aktualisierung des DNS vom ISP.

Überprüfen Sie die DNS-Informationen von dem Computer, auf dem Sie versuchen, mit dem nslookup-Befehlszeilentool auf Ihr Gerät zuzugreifen:

nslookup [Gerätename].syncloud.it

#### Wenn Sie eine falsche IP sehen

Möglicherweise möchten Sie Ihren DNS-Server auf 8.8.8.8 (Google DNS) umstellen.

Testen Sie es zuerst:

nslookup [Gerätename].syncloud.it 8.8.8.8

#### Wenn Sie eine Timeout-Meldung sehen

Wahrscheinlich lässt Ihr Router kein DNS zu, das auf eine lokale IP verweist.

Fritzbox erlaubt zum Beispiel das Hinzufügen einer Ausnahme: https://en.avm.de/service/fritzbox/fritzbox-7390/knowledge-base/publication/show/663_No-DNS-resolution-of-private-IP-addresses/

#### DNS-Problem des Telefons

Installieren Sie die DNS-App DNSDig auf Android oder Deep Dig auf dem iPhone

Geben Sie Ihren Domainnamen ein und erhalten Sie IP. Dadurch erfahren Sie, ob Ihr lokaler DNS-Anbieter gut ist oder ob Sie beispielsweise auf 8.8.8.8 (dns.google) wechseln müssen.

Wenn Sie nicht wissen, wie Sie DNS auf Ihrem Telefon umstellen, kann Google Ihnen helfen.

### Externer Zugriff ist aktiviert

Einige Router unterstützen den Zugriff auf Geräte im lokalen Netzwerk über ihre externe Router-IP-Adresse (NAT Loopback) nicht. Weitere Details hier: https://en.m.wikipedia.org/wiki/Hairpinning

Möglicherweise müssen Sie einen besseren Router mit dieser Funktion kaufen.

Sie können Ihren Router hier überprüfen: http://opensimulator.org/wiki/NAT_Loopback_Routers

Oder googeln Sie: [Name und Modell Ihres Routers] nat loopback

#### Brückenmodus

Manchmal möchten Sie vielleicht Ihren neuen Router mit NAT-Loopback-Funktion vor den Router Ihres Providers stellen, wenn Sie ihn nicht einfach ersetzen können. In diesem Fall müssen Sie den Router des Providers zuerst in einen Bridge-Modus versetzen und dann kann Ihr interner Router eine öffentliche IP erhalten.

https://kb.netgear.com/000028987/When-to-to-put-modem-into-bridge-mode
