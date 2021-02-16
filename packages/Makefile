all: default

orange-pi-plus-2e:
	$(MAKE) packages BOOT_PACKAGES="linux.opiplus2e"

orange-pi-pc-plus:
	$(MAKE) packages BOOT_PACKAGES="linux.opipcplus"

terasic-de10-standard:
	$(MAKE) packages BOOT_PACKAGES="linux.terasicde10standard"

raspberry-pi-3-b:
	$(MAKE) packages BOOT_PACKAGES="linux.rpi3b"

amlogic-s905x:
	$(MAKE) packages BOOT_PACKAGES="linux.amlogics905x"

aws:
	$(MAKE) packages BOOT_PACKAGES="linux.aws"

qemu-kvm64:
	$(MAKE) packages BOOT_PACKAGES="linux.kvm64"

qemu-phenom:
	$(MAKE) packages BOOT_PACKAGES="linux.phenom"

qemu-core2duo:
	$(MAKE) packages BOOT_PACKAGES="linux.core2duo"

qemu-nehalem:
	$(MAKE) packages BOOT_PACKAGES="linux.nehalem"

qemu-westmere:
	$(MAKE) packages BOOT_PACKAGES="linux.westmere"

qemu-sandybridge:
	$(MAKE) packages BOOT_PACKAGES="linux.sandybridge"

qemu-skylake:
	$(MAKE) packages BOOT_PACKAGES="linux.skylake"

p4-630:
	$(MAKE) packages BOOT_PACKAGES="linux.p4-630"

core2duo-q9550:
	$(MAKE) packages BOOT_PACKAGES="linux.core2duo-q9550"

i3-540:
	$(MAKE) packages BOOT_PACKAGES="linux.i3-540"

i5-3317u:
	$(MAKE) packages BOOT_PACKAGES="linux.i5-3317u"

i5-8500:
	$(MAKE) packages BOOT_PACKAGES="linux.i5-8500"

i7-2600:
	$(MAKE) packages BOOT_PACKAGES="linux.i7-2600"

x4-945:
	$(MAKE) packages BOOT_PACKAGES="linux.x4-945"

e2-6110:
	$(MAKE) packages BOOT_PACKAGES="linux.e2-6110"

xeon-5130:
	$(MAKE) packages BOOT_PACKAGES="linux.xeon-5130"

xeon-e5504:
	$(MAKE) packages BOOT_PACKAGES="linux.xeon-e5504"

xeon-e5620:
	$(MAKE) packages BOOT_PACKAGES="linux.xeon-e5620"

xeon-x5650:
	$(MAKE) packages BOOT_PACKAGES="linux.xeon-x5650"

xeon-e3-1271:
	$(MAKE) packages BOOT_PACKAGES="linux.xeon-e3-1271"

lenovo-t460s:
	$(MAKE) packages BOOT_PACKAGES="linux.lenovo-t460s"

BASE_PACKAGES = dahdi libpri libedit jansson sqlite libsrtp asterisk firewall

libpri: dahdi
asterisk: libpri libedit jansson sqlite libsrtp

include Makefile.common
