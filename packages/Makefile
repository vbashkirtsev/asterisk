all: packages

BASE_PACKAGES = dahdi libpri libedit jansson sqlite asterisk

libpri: dahdi
asterisk: libpri libedit jansson sqlite

include Makefile.common
