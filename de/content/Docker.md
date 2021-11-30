```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Docker) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Docker.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Docker.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Docker.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Docker.md) | 

# Docker

Um Syncloud-Image unter Docker auszuführen, verwenden Sie den folgenden Befehl:

### Docker vorbereiten

Stellen Sie sicher, dass Sie systemd cgroupdriver verwenden

Bearbeiten: ```/etc/docker/daemon.json```

```
{
  "exec-opts": ["native.cgroupdriver=systemd"]
}
```

Neu starten:

```
sudo systemctl docker neu starten
```

Andernfalls funktioniert der Container nach dem Neustart nicht und Sie sehen in Ihrem /var/log/syslog Folgendes:

```
Kernel: systemd[1]: Fehler beim Anhängen von 1 an compat systemd cgroup /docker/.../init.scope: No such file or directory
Kernel: systemd[1]: Fehler beim Öffnen der Pin-Datei: Keine solche Datei oder kein Verzeichnis
Kernel: systemd[1]: Manager-Objekt konnte nicht zugewiesen werden: Keine solche Datei oder kein solches Verzeichnis
Kernel: systemd[1]: Ausführung einfrieren.
```

### Syncloud-Container starten

```
Docker ausführen \
  --restart=immer \
  --name=syncloud \
  --volume=/storage:/opt/disk/internal \
  --privilegiert \
  --detach=wahr \
  --publish=443:443 \
  --publish=80:80 \
  syncloud/platform-buster-amd64:21.10
```

Wobei /storage ein Verzeichnis auf Ihrem Host mit ext4-Dateisystem ist

Architekturen:

1. Plattform-Buster-amd64
2. Plattform-Buster-Arm
3. Plattform-Buster-Arm64

Es sollte auf jedem Linux-Betriebssystem mit installiertem Docker funktionieren.

Öffnen Sie https://localhost (oder https://[IP Ihres Docker-Computers]) in Ihrem Browser und folgen Sie dem Aktivierungsverfahren.
