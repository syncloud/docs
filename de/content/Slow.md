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

Sometimes device can be slow to load pages or apps can be unresponsive.

There are few checks you can do to find a solution.

#### Address

Try to open device web using different urls and compare the speed.

* Domain address (ex: bob.syncloud.it)
* Public address (ex: 111.111.111.111)
* Internal address (ex: 192.168.0.1)

Also compare the speed of web loading inside your network (with WiFi) and outside (no WiFI on mobile phone).

All URLs can be found at https://www.syncloud.it

This can can help us identifying the issue for example:

* Domain is wrong or not updating
* Router is slowing down the traffic

#### Device

Run this command on the device using SSH:

```
top -n 1
```

It should show you something like this where we look at key metrics:

* MiB Mem
* avail Mem
* %Cpu(s)

```
top - 14:22:04 up 1 day, 16:38,  1 user,  load average: 0.20, 0.96, 1.21
Tasks: 202 total,   1 running, 201 sleeping,   0 stopped,   0 zombie
%Cpu(s):  0.0 us,  0.0 sy,  0.0 ni, 99.9 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
MiB Mem :   1994.6 total,   1250.1 free,    340.1 used,    404.3 buff/cache
MiB Swap:      0.0 total,      0.0 free,      0.0 used.   1575.8 avail Mem 

  PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND                                                                                                                                        
26723 root      20   0    6832   2304   1800 R   0.3   0.1   0:00.07 top                                                                                                                                            
    1 root      20   0   32060   6044   3436 S   0.0   0.3   0:18.12 systemd                                                                                                                                        
    2 root      20   0       0      0      0 S   0.0   0.0   0:00.02 kthreadd                                                                                                                                       
    4 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker/0:0H                                                                                                                                   
    6 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mm_percpu_wq                                                                                                                                   
    7 root      20   0       0      0      0 S   0.0   0.0   0:00.42 ksoftirqd/0                                                                                                                                    
    8 root      20   0       0      0      0 I   0.0   0.0   0:11.47 rcu_preempt                                                                                                                                    
    9 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_sched                                                                                                                                      
   10 root      20   0       0      0      0 I   0.0   0.0   0:00.00 rcu_bh
```

### Netzwerk

Run this command on the device using SSH:

```
ping google.com -c 5 
```

It will show something like this where we look at:

* time

```
PING google.com (216.58.204.78) 56(84) bytes of data.
64 bytes from lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=1 ttl=116 time=6.05 ms
64 bytes from lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=2 ttl=116 time=6.00 ms
64 bytes from lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=3 ttl=116 time=6.39 ms
64 bytes from lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=4 ttl=116 time=5.89 ms
64 bytes from lhr25s13-in-f14.1e100.net (216.58.204.78): icmp_seq=5 ttl=116 time=6.16 ms

--- google.com ping statistics ---
5 packets transmitted, 5 received, 0% packet loss, time 9ms
rtt min/avg/max/mdev = 5.893/6.096/6.387/0.194 ms
```
