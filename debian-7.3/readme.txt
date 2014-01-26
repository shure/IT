
Debian 7.3 32 bits.

==============================================================

Inslall NIS:

Copy all other files from "etc" to their places.

$ apt-get install portmap nis autofs

Approve all questions.
Reboot.
Home and users should be available.

==============================================================

apt-get -y install git-core tclsh pidgin libsdl-dev apt-file build-essential libc6-dev-amd64 gdb emacs libxp6 libxp-dev

(cd /usr/include/gnu/; cp stubs-64.h stubs-32.h)

==============================================================

For xemacs:
Use xemacs/super.el script for defining SUPER key.
