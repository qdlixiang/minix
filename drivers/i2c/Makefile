# Makefile for I2C support

PROG=   i2c

.include "arch/${MACHINE_ARCH}/Makefile.inc"

SRCS+=   i2c.c

DPADD+= ${LIBCHARDRIVER} ${LIBSYS} ${LIBTIMERS} ${CLKCONF}
LDADD+= -lchardriver -lsys -ltimers -lclkconf

MAN=

BINDIR?= /usr/sbin

CPPFLAGS+= -I${.CURDIR} -I${.CURDIR}/arch/${MACHINE_ARCH}

.include <minix.service.mk>
.include <bsd.subdir.mk>

