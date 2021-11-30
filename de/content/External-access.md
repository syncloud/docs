```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/External-access) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/External-access.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/External-access.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/External-access.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/External-access.md) | 

# Externer Zugang

Der externe Zugriff kann im Abschnitt Einstellungen - Zugriff aktiviert werden.

### Automatikmodus (nicht stabil)

Der einfachste Weg, den externen Zugriff zu aktivieren, besteht darin, die automatische IP-Erkennung und die automatische Portzuordnung einzustellen und zu speichern.

Wenn UPnP auf Ihrem Router aktiviert ist, sollten Sie Portzuordnungen automatisch für Sie erstellen lassen.

Wenn Sie Standardports (80 und 443) erstellt haben, sind Sie gut, andernfalls müssen Sie möglicherweise den manuellen Portzuordnungsmodus verwenden.

### Manuelle Portzuordnung (empfohlen)

Falls UPnP auf dem Router nicht verfügbar ist oder nicht standardmäßige Ports erstellt, müssen Sie die Portzuordnungen manuell auf Ihrem Router erstellen.

Folgen Sie der Dokumentation für Ihren Router. Normalerweise ist es sehr intuitiv, einfach die Webseite Ihres Routers zu öffnen.

Sie müssen zwei Portzuordnungen erstellen:

Router-Port 80 -> Geräte-Port 80, TCP

Router-Port 443 -> Geräte-Port 443, TCP

Viele Router verwenden das Antragsformular unter den Firewall-Einstellungen. Sie sollten eine Anwendung (Syncloud) mit den obigen beiden Portzuordnungen erstellen und sie dann Ihrem Syncloud-Gerät zuweisen. Danach sollten Sie in der Lage sein, den externen Zugriff zu aktivieren.

### Manuelle IP

Die automatische IP-Erkennung ermöglicht es dem DNS-Server, die Quell-IP-Adresse der DNS-Aktualisierungsanforderung zu verwenden.

In seltenen Fällen ist es nicht Ihre öffentliche IP, dann müssen Sie sie manuell angeben.

### Nicht standardmäßige Ports

Der Standard-Port für die Zertifikatsvalidierung ist 80. Wenn er auf Ihrem Router-Gerät nicht verfügbar ist, kann er kein echtes Zertifikat vom Let's Encrypt-Dienst abrufen. Das ist ihre Forderung. Der Browser kann die Gültigkeit Ihres Servers nicht überprüfen.

Der Standardzugriffsport ist 443 (HTTPS). Wenn dieser Port auf Ihrem Router nicht verfügbar ist, können Sie von einigen Netzwerken mit strengen Firewall-Regeln möglicherweise nicht auf Ihr Gerät zugreifen.

### Öffentliche IP (IPv4) auf dem Gerät

Wenn Sie eine öffentliche IP haben, müssen Sie den externen Zugriff nicht aktivieren, da Ihr Gerät bereits aus dem Internet sichtbar ist.

### IPv6 auf dem Gerät

Wenn Sie IPv6 verwenden, ist es per Definition öffentlich und Sie müssen keinen externen Zugriff aktivieren.

Sie können nur über IPv6-Netzwerke auf Ihr Gerät zugreifen.

Um von jedem Netzwerk aus auf Ihr Gerät zugreifen zu können (bis alle auf IPv6 migriert sind), müssen Sie Ihren Provider bitten, Ihnen die öffentliche IPv4-Adresse (für Ihren Router) zu geben und den IPv4-Modus für Ihr Gerät (an Ihrem Router) zu aktivieren. Danach sollten Sie in der Lage sein, den externen Zugriff zu aktivieren.

### DNS-Rebind-Schutz

Wenn Sie eine dynamische IP haben, müssen Sie Ihrem Browser möglicherweise eine Ausnahme für syncloud.it (oder Ihre benutzerdefinierte Domain) hinzufügen, damit die alte Adresse nicht zwischengespeichert wird.
