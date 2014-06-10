
Debian 7.3 32 bits.

==============================================================

Inslall NIS:

Copy all other files from "etc" to their places.

$ apt-get install portmap nis autofs

Approve all questions.
Reboot.
Home and users should be available.

==============================================================

apt-get -y install git-core tcsh pidgin libsdl-dev apt-file build-essential libc6-dev-amd64 gdb emacs libxp6 libxp-dev

(cd /usr/include/gnu/; cp stubs-64.h stubs-32.h)

==============================================================

NVidia driver install:

Add the following line to /etc/apt/sources.list:
deb http://http.debian.net/debian/ wheezy main contrib non-free

aptitude update
aptitude -r install linux-headers-$(uname -r|sed 's,[^-]*-[^-]*-,,') nvidia-kernel-dkms
mkdir /etc/X11/xorg.conf.d
echo -e 'Section "Device"\n\tIdentifier "My GPU"\n\tDriver "nvidia"\nEndSection' > /etc/X11/xorg.conf.d/20-nvidia.conf

reboot

==============================================================


For xemacs:
Use xemacs/super.el script for defining SUPER key.
