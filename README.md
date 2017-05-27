# UFW-Home-Server-Apps

Download appprofiles and put files in /etc/ufw/applications.d, 
```
git clone git@github.com:NathanTheGr8/UFW-Home-Server-Apps.git
sudo cp UFW-Home-Server-Apps/app-profiles/* /etc/ufw/applications.d
```

then tell ufw to reload the application definitions with

```
sudo ufw app update plexmediaserver
sudo ufw app info plexmediaserver
```
Use it with something like:
```
sudo ufw allow plexmediaserver
```