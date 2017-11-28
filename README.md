# etc_openhab2
Configuration directory of my personal /etc/openhab2 directory

On iMac:
edit with Eclipse SmartHome Designer in ~/gitrepos/etc_openhab2
git add *
git commit
git push

Connect to openhab system (raspberry):
Terminal, ssh pi@192.168.2.9
cd ~/gitrepos/etc_openhab2
su
git pull
cp -a * /etc/openhab2

I edit the /etc/openhab2 files (on openhab2 server, raspberry) and then
in ~/gitrepos/etc_openhab2 directory.
cp -a /etc/openhab2 . in
git add *
git commit
git push

.
