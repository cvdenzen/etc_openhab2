# etc_openhab2
Configuration directory of my personal /etc/openhab2 directory

On iMac:
edit with Eclipse SmartHome Designer in ~/gitrepos/etc_openhab2 (or other, but make sure you push changes)
git add *
git commit
git push

Connect to openhab system (raspberry):
Terminal, ssh pi@192.168.2.9
sudo -s -E -u openhab
cd ~/gitrepos/etc_openhab2
(of git clone https://github.com/cvdenzen/etc_openhab2.git)
git pull
cp -a openhab2/* /etc/openhab2
service openhab2 restart (niet nodig, ziet openhab vanzelf?)

I edit the /etc/openhab2 files (on openhab2 server, raspberry) and then
in ~/gitrepos/etc_openhab2 directory.
cp -a /etc/openhab2 .
git add *
git commit
git push

openhab2 karaf:
/usr/share/openhab2/runtime/bin/client
user openhab ww habopen

feature:list|grep bla
feature:install

pilight jar gevonden op https://www.versioneye.com/java/org.openhab.binding:org.openhab.binding.pilight/1.9.0.b3
