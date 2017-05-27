```
[plexmediaserver]
title=Plex Media Server
description=The Plex Media Server is smart software that makes playing Movies, TV Shows and other media on your computer simple
ports=32400/tcp|1900/udp|32469/udp|5353/udp

[sonarr]
title=Sonarr
description=Sonarr is a PVR for Usenet and BitTorrent users
ports=8989/tcp|8989/udp

[radarr]
title=Radarr
description=Radarr is an independent fork of Sonarr reworked for automatically downloading movies via Usenet and BitTorrent.
ports=7878/tcp|7878/udp

[nzbget]
title=NzbGet
description=NZBGet is a binary downloader, which downloads files from Usenet based on information given in nzb-files.
ports=6789/tcp|6789/udp

[deluge]
title=Deluge
description=Deluge is a lightweight, Free Software, cross-platform BitTorrent client.
ports=8112/tcp|8112/udp
```
Once you have defined your application file, put it in /etc/ufw/applications.d, then tell ufw to reload the application definitions with
```
ufw app update plexmediaserver
ufw app info plexmediaserver
```
Use it with something like:
```
ufw allow plexmediaserver
```