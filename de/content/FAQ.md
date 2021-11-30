```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/FAQ) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/FAQ.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/FAQ.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/FAQ.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/FAQ.md) | 

# FAQ

1. Was ist der Unterschied zwischen einer Geräte-App und einer Client-App?

    Alle Cloud-Apps (Gmail, Dropbox ...) bestehen aus zwei Teilen Server (Gerät) und Client (Mobil, Desktop). Server enthält die gesamte Logik und ist viel komplexer zu erstellen und auszuführen. Client ist eine App, die von einem Benutzer verwendet wird, um mit dem Server zu interagieren.

2. Welche Verschlüsselung wird verwendet:

    Das Gerät verwendet immer https, sodass die Verbindung zwischen Ihnen und dem Gerät verschlüsselt ist. Gerätedaten selbst sind nicht verschlüsselt, daher sollten Sie nicht vertrauenswürdigen Personen keinen physischen Zugriff gewähren.

3. Wofür wird eine Micro-SD-Karte verwendet?

    Es wird zum Booten des Geräts (Bootpartition) verwendet, da die meisten Armgeräte nicht direkt von USB oder SATA booten können. Es wird auch als interne Festplatte verwendet (es sei denn, Ihr Gerät ist mit einer internen SSD-Festplatte ausgestattet), die Systemdateien enthält und ein Standarddateispeicher für die Apps ist. Dateispeicherlaufwerk kann in den Speichereinstellungen ausgewählt werden und es kann jeweils nur ein Laufwerk verwendet werden.

4. Externe Festplatte (Dateispeicher).

    Syncloud bietet Dateispeicher für alle Apps und befindet sich standardmäßig auf der internen Festplatte. Benutzer können den Speicherort der Datei zwischen interner oder externer Festplatte im Abschnitt mit den Speichereinstellungen auswählen. Darüber hinaus ermöglichen Apps wie Nextcloud das Anhängen von zusätzlichem externen Speicher.
