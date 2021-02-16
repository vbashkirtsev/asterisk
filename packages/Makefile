all: packages

BASE_PACKAGES = tcpdump dahdi libpri libedit jansson sqlite libsrtp asterisk

tcpdump: libpcap
libpri: dahdi
asterisk: libpri libedit jansson sqlite libsrtp

include Makefile.common
