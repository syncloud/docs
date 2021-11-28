```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/App-porting-guide) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/App-porting-guide.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/App-porting-guide.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/App-porting-guide.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/App-porting-guide.md) | 

# Anleitung zur App-Portierung

Wir führen eine modifizierte [Snapd]()-Instanz auf dem Gerät aus (https://github.com/syncloud/snapd)

### Syncloud Snapd-Unterschiede

* Syncloud Store-Unterstützung
* Weitere Systemparameter
* Keine Einschränkungen (begrenzen, apparmor)

### Unterschiede bei der Erstellung von Syncloud Snap-Paketen

* Keine Begrenzungs- / Apparmor-Definitionen erforderlich
* Wir versuchen, vorgefertigte Binärdateien für komplexe Abhängigkeiten wie Sprachen oder Datenbanken wiederzuverwenden
* Wir verwenden kein Snapcraft-Tool und nur eine einfache build.sh, um die benötigten Abhängigkeiten herunterzuladen/zu kompilieren.

Apps sind übliche Snaps plus Syncloud-spezifische Konfigurations-Snap-Hooks.

### Vor der Portierung

Idealerweise sollte die App über eine Weboberfläche und eine Möglichkeit zur Authentifizierung gegen LDAP verfügen. Die LDAP-Authentifizierung kann von Syncloud für ein App-Projekt implementiert werden, wenn sie bereit sind, sie im Upstream zu akzeptieren.

### Beispiele

Jede Syncloud-App kann als Beispiel für den Aufbau einer neuen verwendet werden.

* PHP: https://github.com/syncloud/nextcloud
* Python: https://github.com/syncloud/users
* JavaScript (NodeJS): https://github.com/syncloud/rocketchat

### App-Verzeichnisstruktur:

* bin: Dienststartskripte
* config: App-Konfigurationen
* Hooks: App-Lifecycle-Ereignisse, derzeit haben wir eine Python-Bibliothek für die Interaktion (sie basiert auf http, sodass jede Sprache verwendet werden kann). Hooks umfassen Snap-Ereignisse (Installieren, Konfigurieren, Post-Refresh) und Syncloud-Plattform-Ereignisse (Zugriffsänderung, Speicheränderung)
* snap: Snap-Paketdefinition (Name, Dienste, Befehle)
* Integration: App-Integration und UI-Tests
* build.sh: Skript erstellen
* .drone.jsonnet: CI-Build-Pipeline

### Was in eine App aufgenommen werden sollte

Laut Snap und dem gesunden Menschenverstand müssen Sie alles enthalten, was die App zum Ausführen benötigt, und es sollte von nichts außer der Kernel-API abhängen. Dazu gehören Datenbanken, Webserver, Caches usw. Dies ermöglicht es uns, Apps jederzeit sicher zu aktualisieren, um ein Update oder eine neuere Version zu erhalten. In Zukunft werden alle Linux-Distributionen so organisiert sein.

### Ein Paket lokal erstellen

Build script bringt alle abhängigen Dienste (Datenbank, Sprache ...) an die richtigen Stellen und erstellt ein einzelnes Archiv mit einem squashfs (app-[version].snap), das Sie später auf dem Gerät installieren oder in unserem Store veröffentlichen können jeder zu benutzen.

### Build erstellen

Wir verwenden den Drone CI-Build-Server für automatisierte Builds mit High-Level-Schritten (Pipeline), die in .drone.jsonnet definiert sind

```
sudo /path/to/cli/drone exec --pipeline=[amd64|arm|arm64] --trusted
```

### Installieren Sie ein Paket auf einem Gerät

```
snap install --devmode /path/to/package.snap
```

### Update-Version

Im Laufe der Zeit müssen Sie Versionen der Upstream-App aktualisieren und Syncloud-Snaps neu verpacken. Gehen Sie dazu wie folgt vor:

1. Ändern Sie die VERSION-Variable in build.sh
2. build-Paket, das alle erforderlichen Tests ausführt
3. Paket auf Ihrem Gerät installieren
4. Erstellen Sie einen PR (Pull Request), damit wir ihn überprüfen und für die Store-Veröffentlichung akzeptieren können
