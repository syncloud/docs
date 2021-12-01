```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Nextcloud) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Nextcloud.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Nextcloud.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Nextcloud.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Nextcloud.md) | 

# Nextcloud

## Befehlszeilentool (occ)

```
Snap-Run nextcloud.occ
```

### Vorschaugenerator

```
snap run nextcloud.occ preview:generate-all -vvv
```

## Große vorhandene Dateisammlungen

Verwenden Sie Nextcloud Client, um Ihre lokalen Dateien mit dem Nextcloud-Gerät zu synchronisieren. Dies kann einige Zeit dauern.

## Datei-Scan

Wenn Sie sich entscheiden, eine Festplatte mit vorhandenen Dateien an Syncloud anzuhängen, stellen Sie sicher, dass sie sich im richtigen Verzeichnis befinden: /nextcloud/[user]/files Dann an Syncloud-Gerät anhängen und in den Speichereinstellungen aktivieren.

Scannen Sie Dateien in Nextcloud, indem Sie diesen Befehl auf dem Gerät ausführen:

```
snap run nextcloud.occ files:scan --all
```

## Papierkorbbereinigung

Dadurch werden alle gelöschten Dateien dauerhaft entfernt. Es ist auch eine Problemumgehung für Papierkorbprobleme, wenn Nextcloud über vorhandene gelöschte Dateien im Benutzerspeicherverzeichnis installiert wird.

```
snap run nextcloud.occ trashbin:cleanup --all-users
```

## Datenbank

Um eine Datenbank-Shell einzugeben, verwenden Sie den folgenden Befehl:

```
Snap run nextcloud.psql
```

## Kalender/Kontakte exportieren

```
cd /tmp
git-Klon https://codeberg.org/BernieO/calcardbackup.git
CD-Calcard-Backup
mkdir-Backup
sudo chown -R nextcloud:nextcloud .
sudo -u nextcloud PATH="${PATH}:/snap/bin" ./calcardbackup /var/snap/nextcloud/current/nextcloud -p -o backup
```

## Administratorrechte beheben

```
snap run nextcloud.psql -c "update oc_ldap_group_mapping set owncloud_name = 'admin'"

snap run nextcloud.psql -c "update oc_ldap_group_members set owncloudname = 'admin'"
```

## Upgrade von der Benutzeroberfläche nicht möglich

Wenn Sie für die Nextcloud-App mehr als eine Version überspringen, müssen Sie die folgenden Befehle bis zum Ende der Liste ausführen, beginnend mit der Version neben Ihrer aktuellen. Wenn Sie beispielsweise v17 verwenden, müssen Sie Befehle ab Version 18 ausführen und bis zum Ende fortfahren.

Um die Befehle auszuführen, verwenden Sie SSH

Version 15

```
wget apps.syncloud.org/apps/nextcloud_19102646_$(dpkg --print-architecture).snap

snap install nextcloud_19102646_$(dpkg --print-architecture).snap --devmode
```

Version 16

```
wget apps.syncloud.org/apps/nextcloud_19111297_$(dpkg --print-architecture).snap

snap install nextcloud_19111297_$(dpkg --print-architecture).snap --devmode
```

Version 17

```
wget apps.syncloud.org/apps/nextcloud_200109121_$(dpkg --print-architecture).snap

snap install nextcloud_200109121_$(dpkg --print-architecture).snap --devmode
```

Version 18

```
wget apps.syncloud.org/apps/nextcloud_200414143_$(dpkg --print-architecture).snap

snap install nextcloud_200414143_$(dpkg --print-architecture).snap --devmode
```

Version 19

```
wget apps.syncloud.org/apps/nextcloud_200724171_$(dpkg --print-architecture).snap

snap install nextcloud_200724171_$(dpkg --print-architecture).snap --devmode
```

Version 20

```
wget apps.syncloud.org/apps/nextcloud_210214199_$(dpkg --print-architecture).snap

snap install nextcloud_210214199_$(dpkg --print-architecture).snap --devmode
```

Version 21

```
wget apps.syncloud.org/apps/nextcloud_210624280_$(dpkg --print-architecture).snap

snap install nextcloud_210624280_$(dpkg --print-architecture).snap --devmode
```

Version 22

```
wget apps.syncloud.org/apps/nextcloud_211101376_$(dpkg --print-architecture).snap

snap install nextcloud_211101376_$(dpkg --print-architecture).snap --devmode
```

Neueste

```
Snap Refresh nextcloud --channel=stable
```
