
Ubuntu-12 32 bits.

==============================================================

Inslall NIS:

Install ubuntu by default and log in as root.
Copy this directory (using scp -r) to /root.

$ apt-get purge network-manager

Copy "etc/network/interfaces" file into /etc/network.

This disables "network manager" temporarily.

Reboot. Network should be available.
Log in again as root in text mode.
Copy all other files from "etc" to their places.

$ apt-get install portmap nis autofs

Approve all questions.
Reboot. Home and users should be available.
Graphical log in should be available.

==============================================================

Other install for RND:

apt-get install gnome
Select "gdm" as greeter screen.

apt-get -y install gnome-tweak-tool gconf-editor 
apt-get -y install apt-file build-essential
apt-get -y install libbfd-dev  libc6-dev libext-dev  libsdl-dev
apt-get -y install libsm-dev  libxaw6-dev libxaw7-dev libxext-dev
apt-get -y install libxmu-dev libxpm-dev libxtst-dev libxp-dev libtiff-dev
apt-get -y install p7zip-full
apt-get -y install vncviewer
apt-get -y install xemacs21
apt-get -y install git-core cvs
apt-get -y remove overlay-scrollbar

Then (as root again):
cd /usr/lib; ln -s i386-linux-gnu/* .

==============================================================

Graphics hacks:

Select "Gnome no effects" in "Session selector". This allows VNC to
work faster (Or altenatively Ununtu no effects).

Use "gnome-tweak-tool" to use "Crux" windows theme to increase window
border width.
