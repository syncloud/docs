```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Mail) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Mail.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Mail.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Mail.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Mail.md) | 

# Mail

## Die Anschrift

Wenn Sie die Mail-App installieren, können Sie E-Mails mit der folgenden Adresse senden und empfangen: [Benutzer]@[Domänenname].syncloud.it

## Email schicken

Sie sollten in der Lage sein, E-Mails von Roundcube aus zu senden.

In seltenen Fällen kann Ihr Internetanbieter den ausgehenden Port 25 blockieren. Verwenden Sie den folgenden Befehl, um zu überprüfen, ob Sie eine Zeitüberschreitung erhalten, die bedeutet, dass der ausgehende Port 25 blockiert ist.

```
nc -vz gmail-smtp-in.l.google.com 25
```

Höchstwahrscheinlich wird Ihre E-Mail im Spam landen, also überprüfen Sie den Spam-Ordner und markieren Sie sie als Nicht-Spam. Gmail zum Beispiel ist sehr aggressiv gegenüber Spam, Yahoo nicht.

## E-Mail empfangen

Sie sollten ein Mapping für Port 25 erstellen (Router-Port 25 -> Geräte-Port 25)

Auf diese Weise können Sie E-Mails empfangen, die an Ihre Geräte-E-Mail gesendet werden.

## Mail-Apps

Während Sie mit der Standard-Weboberfläche alles tun können, was Sie brauchen, können Sie alternative E-Mail-Apps verwenden. Sie können eigenständige E-Mail-Apps (wie K-9 Mail) verwenden, um E-Mails über Ihren Syncloud-Mailserver zu lesen und zu senden. Dazu müssen Sie zwei weitere Ports an Ihrem Router öffnen:

Abrufen: 993 (IMAP SSL/TLS)

Senden: 587 (SMTP STARTTLS)

Server: [user].syncloud.it (oder entsprechende benutzerdefinierte Domain)

Benutzer: Benutzername ohne Domänennamenteil.

## SPAM

Wenn Sie eine dynamische IPv4-Adresse verwenden, wird Ihre E-Mail möglicherweise von E-Mail-Anbietern als Spam markiert. In diesem Fall müssen Sie sich ein statisches IPv4 besorgen oder zu einem IPv6-fähigen Internetanbieter wechseln.
