# $FreeBSD: head/usr.sbin/jls/Makefile 275054 2014-11-25 16:57:27Z bapt $

.include <src.opts.mk>

PROG=	jls
MAN=	jls.8
LIBADD=	jail
LDADD=	-lxo

.if ${MK_INET6_SUPPORT} != "no"
CFLAGS+= -DINET6
.endif
.if ${MK_INET_SUPPORT} != "no"
CFLAGS+= -DINET
.endif

.include <bsd.prog.mk>
