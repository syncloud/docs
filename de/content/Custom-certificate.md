```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Custom-certificate) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Custom-certificate.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Custom-certificate.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Custom-certificate.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Custom-certificate.md) | 

# Custom Zertifikat

Wenn Sie ein eigenes Zertifikat haben, können Sie es installieren, indem Sie diese Dateien ersetzen:

```
/var/snap/platform/common/syncloud.crt
/var/snap/platform/common/syncloud.key
```

Webserver neu starten

```
systemctl restart snap.platform.nginx-public 
```
