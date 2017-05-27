# UFW-Home-Server-Apps

Download appprofiles and put files in /etc/ufw/applications.d, then tell ufw to reload the application definitions with

ufw app update plexmediaserver
ufw app info plexmediaserver
Use it with something like:

ufw allow plexmediaserver
