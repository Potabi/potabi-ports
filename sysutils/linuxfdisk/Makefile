# Created by: netch@netch.kiev.ua

PORTNAME=	linuxfdisk
PORTVERSION=	2.11z
PORTREVISION=	1
CATEGORIES=	sysutils
MASTER_SITES=	KERNEL_ORG/linux/utils/util-linux/v2.11/ \
		http://ftp.be.debian.org/pub/linux/utils/util-linux/v2.11/ \
		ftp://segfault.kiev.ua/pub/
DISTNAME=	util-linux-${PORTVERSION}

MAINTAINER=	netch@netch.kiev.ua
COMMENT=	Fdisk, a partition tables manipulator, from util-linux

LICENSE=	GPLv2+

WRKSRC=		${WRKDIR}/util-linux-${PORTVERSION}/fdisk
USES=		tar:bzip2
ONLY_FOR_ARCHS=	i386 amd64 armv7 powerpc powerpc64 powerpc64le

pre-patch:
	@${CP} ${FILESDIR}/linuxfdisk-Makefile ${WRKSRC}/Makefile
	@${CP} ${FILESDIR}/linuxfdisk-sys_bsd.c ${WRKSRC}/sys_bsd.c

.include <bsd.port.mk>
