```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Managed-domain) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Managed-domain.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Managed-domain.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Managed-domain.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Managed-domain.md) | 

# Verwaltete Domain

Im Rahmen unserer Premium Services bieten wir einen Managed DNS Service an.

Zum Beispiel besitzen Sie **example.com** bei GoDaddy (oder einem anderen Domain-Registrar) und möchten, dass unsere Geräte-Apps wie **https//nextcloud.example.com** angezeigt werden

Dazu müssen Sie:

1. Abonnieren Sie Premium-Dienste unter https://syncloud.it/account
2. Aktualisieren Sie das System über die Einstellungen - Updates
3. Aktivieren Sie das Gerät mit dem Premium-Plan und geben Sie **example.com** als Gerätenamen ein.
4. Gehen Sie zu https://syncloud.it und kopieren Sie Nameserver unter Ihre Domain.
5. Gehen Sie zum Domain-Registrar-Management-Web und geben Sie Nameserver ein
6. Warten Sie, bis DNS aktualisiert ist (~10 Minuten)
7. Öffnen Sie **https//example.com** in einem Browser und installieren Sie Nextcloud (falls noch nicht installiert)
8. Öffnen Sie **https//nextcloud.example.com** in einem Browser
