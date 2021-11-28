```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Diaspora) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Diaspora.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Diaspora.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Diaspora.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Diaspora.md) | 

# Diaspora

### Administratorrechte

Derzeit unterstützt Diaspora kein LDAP, daher können wir dem Gerätebenutzer nicht erlauben, eine Verbindung herzustellen und Administrator zu sein.

Sie haben selbst einen Benutzer erstellt und ihn vorerst zu einem Admin gemacht.

Um sich zum Administrator zu machen, müssen Sie die Diaspora-Konsole ausführen:

```
snap run diaspora.console
```

Machen Sie sich keine Sorgen über Protokollierungsfehler.

Führen Sie dann einen oder mehrere dieser Befehle mit Ihrem Benutzernamen aus, um die benötigten Rollen hinzuzufügen:

```
Role.add_admin User.where(username: "the_username").first.person
        
Role.add_moderator User.where(username: "the_username").first.person

Role.add_spotlight User.where(username: "the_username").first.person
```

Weitere Informationen: https://wiki.diasporafoundation.org/FAQ_for_pod_maintainers#What_are_roles_and_how_do_I_use_them.3F_.2F_Make_yourself_an_admin_or_assign_moderators

### Diaspora neu starten

```
snap restart diaspora
```
