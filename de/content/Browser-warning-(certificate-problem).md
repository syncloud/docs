```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Browser-warning-(certificate-problem)) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Browser-warning-(certificate-problem).md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Browser-warning-(certificate-problem).md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Browser-warning-(certificate-problem).md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Browser-warning-(certificate-problem).md) | 

# Browser Warnung (Zertifikat Problem)

Das Syncloud-Gerät versucht, ein echtes Zertifikat von Let's Encrypt zu erhalten, um Ihren Browser grün zu halten und die Verbindungssicherheit zu überprüfen.

Echtes Zertifikat kann nur erhalten werden, wenn:

* externer Zugriff ist aktiviert (nur IPv4)
* Geräte-Port 80 ist für das Internet geöffnet, beispielsweise durch Erstellen von Port-Mapping (Router 80 -> Gerät 80).

Aus Sicherheitsgründen ist Port 80 nur für Zertifikatsvalidierungszwecke eingeschränkt und kann nicht geändert werden, da dies von Let's Encrypt CA verlangt wird.

Das Abrufen des Zertifikats kann einige Stunden dauern.

Um die Protokolle anzuzeigen, verwenden Sie Einstellungen -> Support-Seite und senden Sie Protokolle. Standardmäßig werden sie nur an Sie gesendet, es sei denn, Sie enthalten Support.
