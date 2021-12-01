```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Report-problems) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Report-problems.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Report-problems.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Report-problems.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Report-problems.md) | 

# Probleme melden

Normalerweise benötigen wir Protokolle von einem Gerät, um bei Problemen zu helfen.

Sie können sie von der Einstellungsseite aus an uns senden, indem Sie "Kopie an Support senden" aktivieren und auf die Schaltfläche Protokolle senden klicken.

Wenn das aus irgendeinem Grund nicht funktioniert, versuchen Sie, mehr Informationen manuell zu sammeln: Sie müssen diese Befehle mit SSH (bevorzugt, da Sie die Ausgabe in die E-Mail kopieren können) oder HDMI ausführen und die Ausgabe an den Syncloud-Support senden (Support at syncloud.it):

```
df -h
ifconfig
Hostname -I
ping google.com -c1
systemctl status --state=inactive snap.* --no-pager
journalctl -e | Schwanz -100
dmesg | Schwanz -100
IP-Route
tail -200 /var/snap/platform/common/log/uwsgi_public.log
tail -200 /var/snap/platform/common/log/platform.log
```

## SSH

Um die obigen Befehle auszuführen, müssen Sie SSH verwenden, mit dem Sie Befehle auf einem Gerät ausführen und uns die Ausgabe senden können.

Verwenden Sie unter Windows Pytty

Installieren und verbinden Sie sich mit Ihrem Gerät über seine IP-Adresse. Verwenden Sie root als Benutzernamen und Ihr Gerätepasswort, das während der Aktivierung festgelegt wurde. Dann sollten Sie ein Terminalfenster sehen, in dem Sie SSH-Befehle eingeben (oder einfügen) und mit der Eingabetaste ausführen können.

## IP

Die IP-Adresse des Geräts sollte vom Router oder der Ausgabe dieses Befehls auf dem Gerät über den angeschlossenen Bildschirm (HDMI) übernommen werden:

```
Hostname -I
```
