```diff
! Die Übersetzung befindet sich in der Entwicklung. Bitte verlassen Sie sich auf die englische Originalversion.
```

[Seiten](https://github.com/syncloud/docs/blob/master/de/index.md#seiten)

[en](https://github.com/syncloud/platform/wiki/Slow) | 
de | 
[cn](https://github.com/syncloud/docs/blob/master/cn/content/Slow.md) | 
[ru](https://github.com/syncloud/docs/blob/master/ru/content/Slow.md) | 
[fr](https://github.com/syncloud/docs/blob/master/fr/content/Slow.md) | 
[es](https://github.com/syncloud/docs/blob/master/es/content/Slow.md) | 

# Zu langsam

Manchmal kann das Gerät beim Laden von Seiten langsam sein oder Apps reagieren nicht mehr.

Es gibt nur wenige Überprüfungen, die Sie durchführen können, um eine Lösung zu finden.

### Adresse

Versuchen Sie, das Geräte-Web mit verschiedenen URLs zu öffnen und die Geschwindigkeit zu vergleichen.

* Domainadresse (z. B. bob.syncloud.it)
* Öffentliche Adresse (zB: 111.111.111.111)
* Interne Adresse (zB: 192.168.0.1)

Vergleichen Sie auch die Geschwindigkeit des Webladens innerhalb Ihres Netzwerks (mit WLAN) und außerhalb (kein WLAN auf dem Mobiltelefon).

Alle URLs finden Sie unter https://www.syncloud.it

Dies kann uns beispielsweise bei der Identifizierung des Problems helfen:

* Domain ist falsch oder wird nicht aktualisiert
* Router verlangsamt den Datenverkehr

### Gerät

Führen Sie diesen Befehl auf dem Gerät mit SSH aus:

oben -n 1

Es sollte Ihnen ungefähr Folgendes zeigen, wo wir uns die wichtigsten Metriken ansehen:

* MiB-Speicher
* hilf mir
* % CPU(s)

```
top - 14:22:04 up 1 Tag, 16:38, 1 User, Load Average: 0.20, 0.96, 1.21
Aufgaben: 202 insgesamt, 1 läuft, 201 schlafend, 0 gestoppt, 0 Zombie
%Cpu(s): 0.0 us, 0.0 sy, 0.0 ni, 99.9 id, 0.0 wa, 0.0 hi, 0.0 si, 0.0 st
MiB Mem: 1994,6 gesamt, 1250,1 frei, 340,1 verwendet, 404,3 Buff/Cache
MiB-Swap: 0.0 gesamt, 0.0 frei, 0.0 verwendet. 1575.8 verfügbar Mem

  PID USER PR NI VIRT RES SHR S %CPU %MEM TIME+ COMMAND
26723 Wurzel 20 0 6832 2304 1800 R 0,3 0,1 0:00,07 oben
    1 Wurzel 20 0 32060 6044 3436 S 0.0 0.3 0.18.12 systemd
    2 Wurzel 20 0 0 0 0 S 0.0 0.0 0:00.02 kthreadd
    4 Wurzel 0 -20 0 0 0 I 0.0 0.0 0:00.00 kworker/0:0H
    6 Wurzel 0 -20 0 0 0 E 0.0 0.0 0:00.00 mm_percpu_wq
    7 Wurzel 20 0 0 0 0 S 0.0 0.0 0:00.42 ksoftirqd/0
    8 Wurzel 20 0 0 0 0 I 0.0 0.0 0:11.47 rcu_preempt
    9 Wurzel 20 0 0 0 0 E 0.0 0.0 0:00.00 rcu_sched
   10 Wurzel 20 0 0 0 0 I 0.0 0.0 0:00.00 rcu_bh
```

### Netzwerk

Führen Sie diesen Befehl auf dem Gerät mit SSH aus:

```
ping google.com -c 5
```

Es wird ungefähr so ​​​​zeigen, wo wir uns ansehen:

* Zeit

```
PING google.com (216.58.204.78) 56(84) Byte Daten.
64 Byte von lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=1 ttl=116 Zeit=6.05 ms
64 Byte von lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=2 ttl=116 Zeit=6.00 ms
64 Byte von lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=3 ttl=116 Zeit=6,39 ms
64 Byte von lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=4 ttl=116 Zeit=5.89 ms
64 Byte von lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=5 ttl=116 Zeit=6.16 ms

--- google.com Ping-Statistik ---
5 Pakete übertragen, 5 empfangen, 0% Paketverlust, Zeit 9ms
rtt min/avg/max/mdev = 5,893/6,096/6,387/0,194 ms
```
