# Copyright Fivnex, LLC.

PORTNAME= potabi-wallpapers
PORTVERSION=1
CATEGORIES=x11-themes
MAINTAINER=kai@fivnex.co
COMMENT=Wallpapers for Potabi
LICENSE=BSD
USE_GITHUB=yes
GH_ACCOUNT=Potabi
NO_BUILD=yes

do-install:
	${MKDIR} ${STAGEDIR}${PREFIX}/share/backgrounds/optabi
	${CP} -PR ${WRKSRC}/*.jpg ${STAGEDIR}${PREFIX}/share/backgrounds/potabi
	${CP} -PR ${WRKSRC}/*.jpeg ${STAGEDIR}${PREFIX}/share/backgrounds/potabi
	${CP} -PR ${WRKSRC}/*.png ${STAGEDIR}${PREFIX}/share/backgrounds/potabi
	${MKDIR} ${STAGEDIR}${PREFIX}/share/mate-background-properties
	${CP} -PR ${WRKSRC}/ghostbsd.xml ${STAGEDIR}${PREFIX}/share/mate-background-properties

.include <bsd.port.mk>