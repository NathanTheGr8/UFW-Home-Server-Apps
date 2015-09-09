
```
[plexmediaserver]
title=Plex Media Server
description=The Plex Media Server is smart software that makes playing Movies, TV Shows and other media on your computer simple
ports=32400/tcp|1900/udp|32469/udp|5353/udp
```

Once you have defined your application file, put it in 

```/etc/ufw/applications.d```, 

then tell ufw to reload the application definitions with

```
ufw app update plexmediaserver
ufw app info plexmediaserver
```

Use it with something like:

```
ufw allow from 192.168.1.10 to any app plexmediaserver
ufw allow plexmediaserver
```